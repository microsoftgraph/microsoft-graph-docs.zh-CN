---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82311a66c5f8b7744af3170c03a3f2efaaba22f1
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871434"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageByPrinter = await graphClient.Print.Reports.MonthlyPrintUsageByPrinter
    .Request()
    .GetAsync();

```