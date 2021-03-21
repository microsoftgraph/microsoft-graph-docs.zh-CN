---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc9d5c25400c8bf05fa214a5bf14f5b1bee2071e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageByPrinter = await graphClient.Reports.MonthlyPrintUsageByPrinter
    .Request()
    .GetAsync();

```