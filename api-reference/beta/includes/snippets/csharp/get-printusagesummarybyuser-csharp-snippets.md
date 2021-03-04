---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abd20deed7e70ec485b30032d8b328a08db99dca
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441393"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByUser = await graphClient.Print.Reports.DailyPrintUsageSummariesByUser["{id}"]
    .Request()
    .GetAsync();

```