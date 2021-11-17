---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de91f93773bd6181e341ab787d9c8974180cda98
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyCredential = new KeyCredential
{
    Type = "AsymmetricX509Cert",
    Usage = "Verify",
    Key = Convert.FromBase64String("MIIDYDCCAki...")
};

PasswordCredential passwordCredential = null;

var proof = "eyJ0eXAiOiJ...";

await graphClient.Applications["{application-id}"]
    .AddKey(keyCredential,proof,passwordCredential)
    .Request()
    .PostAsync();

```