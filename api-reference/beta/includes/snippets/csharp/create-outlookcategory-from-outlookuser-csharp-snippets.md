---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c508364eaa7b2727b139d26a30b2bc97e732b643
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = new OutlookCategory
{
    DisplayName = "Project expenses",
    Color = CategoryColor.Preset9
};

await graphClient.Me.Outlook.MasterCategories
    .Request()
    .AddAsync(outlookCategory);

```