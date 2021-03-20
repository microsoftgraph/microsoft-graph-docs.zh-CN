---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06c29f8fab6ea8964784af08516b3dac62601943
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948802"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageByPrinter = await graphClient.Reports.DailyPrintUsageByPrinter
    .Request()
    .GetAsync();

```