---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a5020d8334f5b58ca643a85731a4356275f0c67c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465844"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ConvertToRange()
    .Request()
    .PostAsync();

```