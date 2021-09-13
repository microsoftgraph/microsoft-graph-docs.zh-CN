---
title: 生成用于滚动密钥的所有权证明令牌
description: 作为对 addKey 和 removeKey 方法的请求验证的一部分，需要提供所有权证明令牌。 本文档提供生成所有权证明令牌的指南。
ms.localizationpriority: high
ms.prod: applications
author: davidmu1
ms.openlocfilehash: 1df754757ce5707f0c06c709fc3adc423ad36da0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142416"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a>生成用于滚动密钥的所有权证明令牌

可以使用在 [application](/graph/api/resources/application?view=graph-rest-1.0) 和 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) 资源上定义的 **addKey** 和 **removeKey** 方法，以编程方式滚动过期密钥。

作为对这些方法的请求验证的一部分，在调用这些方法之前，将对现有密钥的所有权证明进行验证。 该证明由自签名的 JWT 令牌表示。 此 JWT 令牌必须使用应用程序现有有效证书之一的私钥进行签名。 令牌有效期不应超过 10 分钟。

> **注意：** 没有任何现有有效证书（尚未添加证书，或者所有证书均已过期）的应用程序将无法使用此服务操作。 可改用[更新应用程序](/graph/api/application-update?view=graph-rest-v1.0)操作来执行更新。

令牌应包含以下声明：

- `aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。
- `iss` - 颁发者需要是正在进行调用的应用程序的 Azure AD __ObjectId__（而非 applicationId 或 clientId）。
- `nbf` -“不早于”时间。
- `exp` - 过期时间应该是“不早于”+ 10 分钟。

可使用以下代码示例来生成此所有权证明令牌。

```csharp
using System;
using System.Collections.Generic;
using System.Security.Cryptography.X509Certificates;
using Microsoft.IdentityModel.Tokens;
using Microsoft.IdentityModel.JsonWebTokens;

namespace MicrosoftIdentityPlatformProofTokenGenerator
{
    class Program
    {
        static void Main(string[] args)
        {
            // Configure the following
            string pfxFilePath = "<Path to your certificate file";
            string password = "<Certificate password>";
            string objectId = "<id of the application or servicePrincipal object>";

            // Get signing certificate
            X509Certificate2 signingCert = new X509Certificate2(pfxFilePath, password);

            // audience
            string aud = $"00000002-0000-0000-c000-000000000000";

            // aud and iss are the only required claims.
            var claims = new Dictionary<string, object>()
            {
                { "aud", aud },
                { "iss", objectId }
            };

            // token validity should not be more than 10 minutes
            var now = DateTime.UtcNow;
            var securityTokenDescriptor = new SecurityTokenDescriptor
            {
                Claims = claims,
                NotBefore = now,
                Expires = now.AddMinutes(10),
                SigningCredentials = new X509SigningCredentials(signingCert)
            };

            var handler = new JsonWebTokenHandler();
            var x = handler.CreateToken(securityTokenDescriptor);
            Console.WriteLine(x);
        }
    }
}
```

> **注意：** 可以使用其他工具（如 PowerShell 或使用 Azure KeyVault 的签名）生成证明。 请务必注意，JWT 标头和有效负载中不得包含填充字符“=”，否则将返回 **Authentication_MissingOrMalformed** 错误。
