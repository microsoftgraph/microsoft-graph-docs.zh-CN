---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59394faa9b314914b824064cde79e53f11909ef0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979822"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTrigger printTaskTrigger = new PrintTaskTrigger();
printTaskTrigger.event = PrintEvent.JOB_STARTED;
printTaskTrigger.additionalDataManager().put("definition@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"));

graphClient.print().printers("ae63f617-4856-4b45-8ea9-69dfbeea230e").taskTriggers()
    .buildRequest()
    .post(printTaskTrigger);

```