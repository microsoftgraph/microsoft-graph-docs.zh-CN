---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f7de87de35f95dae687d63d64ba41c65fa94062
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869896"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinter printUsageByPrinter = graphClient.print().reports().dailyPrintUsageByPrinter("016b5565-3bbf-4067-b9ff-4d68167eb1a6")
    .buildRequest()
    .get();

```