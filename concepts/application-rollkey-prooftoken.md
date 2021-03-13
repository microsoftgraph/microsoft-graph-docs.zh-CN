---
title: 生成用于滚动密钥的所有权证明令牌
description: 作为对 addKey 和 removeKey 方法的请求验证的一部分，需要提供所有权证明令牌。 本文档提供生成所有权证明令牌的指南。
localization_priority: Priority
ms.prod: applications
author: davidmu1
ms.openlocfilehash: c459159c780b819589b196dcc44ee0a0cf9a65af
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760831"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a><span data-ttu-id="25ed4-104">生成用于滚动密钥的所有权证明令牌</span><span class="sxs-lookup"><span data-stu-id="25ed4-104">Generating proof of possession tokens for rolling keys</span></span>

<span data-ttu-id="25ed4-105">可以使用在 [application](/graph/api/resources/application?view=graph-rest-1.0) 和 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) 资源上定义的 **addKey** 和 **removeKey** 方法，以编程方式滚动过期密钥。</span><span class="sxs-lookup"><span data-stu-id="25ed4-105">You can use the **addKey** and **removeKey** methods defined on the [application](/graph/api/resources/application?view=graph-rest-1.0) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) resources to roll expiring keys programmatically.</span></span>

<span data-ttu-id="25ed4-106">作为对这些方法的请求验证的一部分，在调用这些方法之前，将对现有密钥的所有权证明进行验证。</span><span class="sxs-lookup"><span data-stu-id="25ed4-106">As part of the request validation for these methods, a proof of possession of an existing key is verified before the methods can be invoked.</span></span> <span data-ttu-id="25ed4-107">该证明由自签名的 JWT 令牌表示。</span><span class="sxs-lookup"><span data-stu-id="25ed4-107">The proof is represented by a self-signed JWT token.</span></span> <span data-ttu-id="25ed4-108">此 JWT 令牌必须使用应用程序现有有效证书之一的私钥进行签名。</span><span class="sxs-lookup"><span data-stu-id="25ed4-108">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="25ed4-109">令牌有效期不应超过 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="25ed4-109">The token lifespan should not exceed 10 minutes.</span></span>

> <span data-ttu-id="25ed4-110">**注意：** 没有任何现有有效证书（尚未添加证书，或者所有证书均已过期）的应用程序将无法使用此服务操作。</span><span class="sxs-lookup"><span data-stu-id="25ed4-110">**Note:** Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="25ed4-111">可改用[更新应用程序](/graph/api/application-update?view=graph-rest-v1.0)操作来执行更新。</span><span class="sxs-lookup"><span data-stu-id="25ed4-111">You can use the [Update application](/graph/api/application-update?view=graph-rest-v1.0) operation to perform an update instead.</span></span>

<span data-ttu-id="25ed4-112">令牌应包含以下声明：</span><span class="sxs-lookup"><span data-stu-id="25ed4-112">The token should contain the following claims:</span></span>

- <span data-ttu-id="25ed4-113">`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</span><span class="sxs-lookup"><span data-stu-id="25ed4-113">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span>
- <span data-ttu-id="25ed4-114">`iss` - 颁发者需要是正在进行调用的应用程序的 Azure AD __ObjectId__（而非 applicationId 或 clientId）。</span><span class="sxs-lookup"><span data-stu-id="25ed4-114">`iss` - Issuer needs to be the Azure AD __ObjectId__  of the application that is making the call (not the applicationId or clientId).</span></span>
- <span data-ttu-id="25ed4-115">`nbf` -“不早于”时间。</span><span class="sxs-lookup"><span data-stu-id="25ed4-115">`nbf` - Not before time.</span></span>
- <span data-ttu-id="25ed4-116">`exp` - 过期时间应该是“不早于”+ 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="25ed4-116">`exp` - Expiration time should be "nbf" + 10 mins.</span></span>

<span data-ttu-id="25ed4-117">可使用以下代码示例来生成此所有权证明令牌。</span><span class="sxs-lookup"><span data-stu-id="25ed4-117">You can use the following code example to generate this proof of possession token.</span></span>

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
