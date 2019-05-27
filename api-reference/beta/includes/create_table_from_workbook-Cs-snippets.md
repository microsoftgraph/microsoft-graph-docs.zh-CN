---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5abcf407f9c89364a8a7b4f5c199a719f4e79845
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "A1:D8";

var hasHeaders = false;

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables
    .Add(address,hasHeaders)
    .Request()
    .PostAsync();

```