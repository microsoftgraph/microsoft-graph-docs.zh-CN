---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4ea549b11fc8a00d9dd07a3fcb4b55db73361ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981500"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinter printUsageByPrinter = graphClient.print().reports().dailyPrintUsageSummariesByPrinter("{id}")
    .buildRequest()
    .get();

```