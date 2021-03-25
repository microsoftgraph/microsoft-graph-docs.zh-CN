---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 866f5448b4ad04fec21925188c7abd58338830fd
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210466"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinterCollectionPage dailyPrintUsageSummariesByPrinter = graphClient.print().reports().dailyPrintUsageSummariesByPrinter()
    .buildRequest()
    .get();

```