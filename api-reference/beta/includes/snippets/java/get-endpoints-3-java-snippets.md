---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0959a03b2656798872d97d984f9ff814e75e67b8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953180"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByPrinterCollectionPage dailyPrintUsageSummariesByPrinter = graphClient.print().reports().dailyPrintUsageSummariesByPrinter()
    .buildRequest()
    .get();

```