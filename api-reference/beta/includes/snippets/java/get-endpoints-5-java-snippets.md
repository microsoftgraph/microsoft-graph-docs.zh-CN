---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b06f8d59dcf0dad96f9b5990a8b29486503f9621
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209321"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinterCollectionPage monthlyPrintUsageSummariesByPrinter = graphClient.print().reports().monthlyPrintUsageSummariesByPrinter()
    .buildRequest()
    .get();

```