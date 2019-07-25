---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef3e4b24b155f3322a01d3d8b99b991ce360e3bf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707346"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    ParentFolderId = "parentFolderId-value",
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders["{id}"]
    .Request()
    .UpdateAsync(contactFolder);

```