---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ba993dd87d7f2812317435ca952278a529ce8e2
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageByUser = await graphClient.Print.Reports.DailyPrintUsageByUser
    .Request()
    .GetAsync();

```