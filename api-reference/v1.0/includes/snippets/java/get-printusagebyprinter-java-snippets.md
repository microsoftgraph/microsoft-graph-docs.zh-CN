---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 352afdf1b4907fa223df2a662e31aa653d6d98bd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974330"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinter printUsageByPrinter = graphClient.reports().dailyPrintUsageByPrinter("{id}")
    .buildRequest()
    .get();

```