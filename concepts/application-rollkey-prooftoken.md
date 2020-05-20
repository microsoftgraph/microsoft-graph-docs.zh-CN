---
title: 为滚动密钥生成已所有权令牌的证明
description: 作为 addKey 和 removeKey 方法的请求验证的一部分，需要使用已拥有令牌的证明。 本文档提供了有关生成已占有令牌证明的指南。
localization_priority: Priority
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 516673b3f5ef318f1c2cc42778d8bec99471c630
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289649"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a>为滚动密钥生成已所有权令牌的证明

您可以使用[应用程序](/graph/resources/application?view=graph-rest-v1.0)上定义的**addKey**和**removeKey**方法和[servicePrincipal](/graph/resources/serviceprincipal?view=graph-rest-v1.0)资源以编程方式滚动过期的项。

作为这些方法的请求验证的一部分，可以在调用方法之前验证现有密钥的所有权证明。 校样由自签名的 JWT 令牌表示。 必须使用应用程序的现有有效证书之一的私钥对此 JWT 令牌进行签名。 令牌寿命不应超过10分钟。

> **注意：** 没有任何现有有效证书的应用程序（尚未添加任何证书，或所有证书已过期）将无法使用此服务操作。 可以使用[更新应用程序](/graph/api/application-update?view=graph-rest-v1.0)操作来改为执行更新。

令牌应包含以下声明：

- `aud`-需要访问群体 `00000002-0000-0000-c000-000000000000` 。
- `iss`-颁发者必须是正在进行呼叫的应用程序的__id__ 。
- `nbf`-不早时间。
- `exp`-过期时间应为 "nbf" + 10 分钟。

您可以使用下面的代码示例生成此已占有令牌的证明。

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
