---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25cd7f11efa4de4004aaf6f0996d613a444bc210
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByPrinter = await graphClient.Print.Reports.DailyPrintUsageByPrinter["{printUsageByPrinter-id}"]
    .Request()
    .GetAsync();

```