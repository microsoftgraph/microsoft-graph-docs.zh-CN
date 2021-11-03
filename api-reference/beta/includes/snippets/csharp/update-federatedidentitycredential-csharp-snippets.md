---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25ce60d69fe5826ea8cff830d46b055533b782f3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var federatedIdentityCredential = new FederatedIdentityCredential
{
    Name = "testing02",
    Issuer = "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    Subject = "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    Description = "Updated description",
    Audiences = new List<String>()
    {
        "api://AzureADTokenExchange"
    }
};

await graphClient.Applications["{application-id}"].FederatedIdentityCredentials["{federatedIdentityCredential-id}"]
    .Request()
    .UpdateAsync(federatedIdentityCredential);

```