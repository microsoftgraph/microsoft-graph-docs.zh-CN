---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a5020d8334f5b58ca643a85731a4356275f0c67c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738274"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ConvertToRange()
    .Request()
    .PostAsync();

```