---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95333213c044da6397a1368dc502bc86d1484856
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771300"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTask printTask = new PrintTask();
PrintTaskStatus status = new PrintTaskStatus();
status.state = PrintTaskProcessingState.COMPLETED;
status.description = "completed";
printTask.status = status;

graphClient.print().taskDefinitions("{taskDefinitionId}").tasks("{taskId}")
    .buildRequest()
    .patch(printTask);

```