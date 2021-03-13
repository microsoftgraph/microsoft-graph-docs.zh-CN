---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb8e3ee6c49bdbd5132216fe17fbf61974823db0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByPrinter = await graphClient.Print.Reports.DailyPrintUsageSummariesByPrinter["{printUsageByPrinter-id}"]
    .Request()
    .GetAsync();

```