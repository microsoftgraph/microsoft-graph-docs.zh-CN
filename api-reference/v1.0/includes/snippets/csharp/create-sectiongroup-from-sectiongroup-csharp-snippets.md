---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa65adfb7d6afde22365edb35ffd9fc680953629
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510152"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = new SectionGroup
{
    DisplayName = "Section group name"
};

await graphClient.Me.Onenote.SectionGroups["{id}"].SectionGroups
    .Request()
    .AddAsync(sectionGroup);

```