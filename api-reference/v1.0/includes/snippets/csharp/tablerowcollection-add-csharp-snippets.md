---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5fd335ea25d62c09fa69f088fc748c133a2bfe21
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838744"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 5;

var values = new List<Json>()
{
    new List<Json>()
{
    1,
    2,
    3
},
    new List<Json>()
{
    4,
    5,
    6
}
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows
    .Add(index,values)
    .Request()
    .PostAsync();

```