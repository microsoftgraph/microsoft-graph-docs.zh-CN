---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d4e9afed0702b922d5a35cd341603cc53f284b5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "id-value";

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Sections["{id}"]
    .CopyToSectionGroup(id,groupId,renameAs,siteCollectionId,siteId)
    .Request()
    .PostAsync();

```