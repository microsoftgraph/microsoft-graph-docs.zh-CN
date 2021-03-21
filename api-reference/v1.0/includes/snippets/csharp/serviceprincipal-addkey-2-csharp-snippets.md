---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b315b157d94135654b0cfb1705188fc34b92456e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyCredential = new KeyCredential
{
    Type = "X509CertAndPassword",
    Usage = "Sign",
    Key = Encoding.ASCII.GetBytes("MIIDYDCCAki...")
};

var passwordCredential = new PasswordCredential
{
    SecretText = "MKTr0w1..."
};

var proof = "eyJ0eXAiOiJ...";

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .AddKey(keyCredential,proof,passwordCredential)
    .Request()
    .PostAsync();

```