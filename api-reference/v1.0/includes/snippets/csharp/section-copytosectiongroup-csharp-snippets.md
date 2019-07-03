---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d4e9afed0702b922d5a35cd341603cc53f284b5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493398"
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