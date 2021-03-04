---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61562eb9f01fcf116f754fecffb49894aeb2e34c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441456"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinter printUsageByPrinter = graphClient.print().reports().dailyPrintUsageSummariesByPrinter("{id}")
    .buildRequest()
    .get();

```