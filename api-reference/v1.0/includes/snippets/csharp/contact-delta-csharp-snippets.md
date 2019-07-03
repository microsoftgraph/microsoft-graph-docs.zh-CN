---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a9c3ee3d03126a4452533aafc3ea9afd69f713a6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{id}"].Contacts.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .Select( e => new {
             e.DisplayName 
             })
    .GetAsync();

```