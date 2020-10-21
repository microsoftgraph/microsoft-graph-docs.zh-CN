---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2526f1bb7aa311714bd51162c3cf2312e15734d9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = new OnenoteSection
{
    DisplayName = "Section name"
};

await graphClient.Me.Onenote.SectionGroups["{id}"].Sections
    .Request()
    .AddAsync(onenoteSection);

```