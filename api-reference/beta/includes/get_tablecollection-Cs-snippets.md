---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b797523f5bd8b20faaf589ecaa45892d2a227907
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445684"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tables = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables
    .Request()
    .GetAsync();

```