---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30ef2d6815e1e0cb2321ffe5e39d0a5516fc260a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageSummariesByPrinter = await graphClient.Print.Reports.MonthlyPrintUsageSummariesByPrinter
    .Request()
    .GetAsync();

```