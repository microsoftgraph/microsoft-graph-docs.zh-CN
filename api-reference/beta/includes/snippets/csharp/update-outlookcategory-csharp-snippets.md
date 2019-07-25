---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 559de4da1e02063845a0b6cbacec576ac3e5f0c4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720954"
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