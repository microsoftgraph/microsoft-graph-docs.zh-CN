---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19de301a23d1162a81a259f6c3b12dbbc7b17157
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = new SectionGroup
{
    DisplayName = "Section group name"
};

await graphClient.Me.Onenote.SectionGroups["{sectionGroup-id}"].SectionGroups
    .Request()
    .AddAsync(sectionGroup);

```