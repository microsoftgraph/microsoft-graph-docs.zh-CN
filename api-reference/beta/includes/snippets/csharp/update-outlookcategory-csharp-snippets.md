---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 559de4da1e02063845a0b6cbacec576ac3e5f0c4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = new OutlookCategory
{
    Color = CategoryColor.Preset15
};

await graphClient.Me.Outlook.MasterCategories["bac262b7-485d-4739-b436-e31467d64fac"]
    .Request()
    .UpdateAsync(outlookCategory);

```