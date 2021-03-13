---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2d335ede71a630466821d9b7adbb950a8e130c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771839"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTrigger printTaskTrigger = new PrintTaskTrigger();
printTaskTrigger.event = PrintEvent.JOB_STARTED;
printTaskTrigger.additionalDataManager().put("definition@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"));

graphClient.print().printers("{printerId}").taskTriggers()
    .buildRequest()
    .post(printTaskTrigger);

```