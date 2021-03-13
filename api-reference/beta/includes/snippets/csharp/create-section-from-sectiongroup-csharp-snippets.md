---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94812ae9a2656f1610de338fd8949e425fbe068b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = new OnenoteSection
{
    DisplayName = "Section name"
};

await graphClient.Me.Onenote.SectionGroups["{sectionGroup-id}"].Sections
    .Request()
    .AddAsync(onenoteSection);

```