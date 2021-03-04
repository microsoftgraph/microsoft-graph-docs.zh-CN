---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dac18d68dd9dfaf407f62f4c3a33b2bbff4f1230
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441392"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUser printUsageByUser = graphClient.print().reports().dailyPrintUsageSummariesByUser("{id}")
    .buildRequest()
    .get();

```