---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e4f7d16293f55c6dc6ca5e725a72222c0e0a4ef
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = new Int32
{
};

var values = new List<Json>()
{
    new Json
    {
    }
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Add(index,values,name)
    .Request()
    .PostAsync();

```