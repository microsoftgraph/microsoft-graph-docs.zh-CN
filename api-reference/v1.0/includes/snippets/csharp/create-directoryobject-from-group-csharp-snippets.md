---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 77c9c9a763ac65e41d90e39948fbdb1ec9352822
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/users/{id}"}
    }
};

await graphClient.Users["{id}"].Manager.Reference
    .Request()
    .PutAsync(directoryObject);

```