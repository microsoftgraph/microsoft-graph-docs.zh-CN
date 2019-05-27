---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 69762d057c18edc282cd217fca59d9610362d806
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calculationType = "calculationType-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Application
    .Calculate(calculationType)
    .Request()
    .PostAsync();

```