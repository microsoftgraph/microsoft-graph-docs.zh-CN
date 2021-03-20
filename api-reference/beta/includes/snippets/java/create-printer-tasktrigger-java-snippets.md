---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 972258a4bd0ead8c3db2cf04d22af405df1a9446
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTrigger printTaskTrigger = new PrintTaskTrigger();
printTaskTrigger.event = PrintEvent.JOB_STARTED;
printTaskTrigger.additionalDataManager().put("definition@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"));

graphClient.print().printers("ae63f617-4856-4b45-8ea9-69dfbeea230e").taskTriggers()
    .buildRequest()
    .post(printTaskTrigger);

```