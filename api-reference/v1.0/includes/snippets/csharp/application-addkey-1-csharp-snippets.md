---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58227998b400029b4d7a5f0e4a6f06aed539a686b35d544b428b3acdbe0bdbf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyCredential = new KeyCredential
{
    Type = "AsymmetricX509Cert",
    Usage = "Verify",
    Key = Encoding.ASCII.GetBytes("MIIDYDCCAki...")
};

PasswordCredential passwordCredential = null;

var proof = "eyJ0eXAiOiJ...";

await graphClient.Applications["{application-id}"]
    .AddKey(keyCredential,proof,passwordCredential)
    .Request()
    .PostAsync();

```