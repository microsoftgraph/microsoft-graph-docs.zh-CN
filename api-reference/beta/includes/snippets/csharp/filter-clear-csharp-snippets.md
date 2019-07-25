---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3dc76a3f9452571f9e28eed9d0be26fecbb0419d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"].Filter
    .Clear()
    .Request()
    .PostAsync();

```