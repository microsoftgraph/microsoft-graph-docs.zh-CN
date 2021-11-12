---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ab004664a6d1b609e2847afe21233411e88dea81e5aad5ced01c8f0ad42d602
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105543"
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