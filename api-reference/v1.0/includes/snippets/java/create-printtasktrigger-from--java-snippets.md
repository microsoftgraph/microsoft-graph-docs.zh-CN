---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fcc2d30dfed1796333704e9d2d529eb28f4fd2a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966716"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTrigger printTaskTrigger = new PrintTaskTrigger();
printTaskTrigger.event = PrintEvent.JOB_STARTED;
printTaskTrigger.additionalDataManager().put("definition@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"));

graphClient.print().printers("{printerId}").taskTriggers()
    .buildRequest()
    .post(printTaskTrigger);

```