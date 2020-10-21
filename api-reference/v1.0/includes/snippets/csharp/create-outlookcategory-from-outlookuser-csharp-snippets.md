---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c508364eaa7b2727b139d26a30b2bc97e732b643
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618729"
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