---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2f8cf0b5352f99f2cf3b701ed3face7fca3591b1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var series = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series
    .Request()
    .GetAsync();

```