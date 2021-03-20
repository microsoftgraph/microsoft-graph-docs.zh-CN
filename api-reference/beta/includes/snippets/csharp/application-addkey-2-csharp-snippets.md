---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa0117b0f4a8b1b922c265b38e4df7306fbcb5d7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942739"
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

await graphClient.Applications["{application-id}"]
    .AddKey(keyCredential,proof,passwordCredential)
    .Request()
    .PostAsync();

```