---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e619915abf25c87555bc58ac0ca4c8420d793ec
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968115"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTask printTask = new PrintTask();
PrintTaskStatus status = new PrintTaskStatus();
status.state = PrintTaskProcessingState.COMPLETED;
status.description = "completed";
printTask.status = status;

graphClient.print().taskDefinitions("3203656e-6069-4e10-8147-d25290b00a3c").tasks("d036638b-1272-4bba-9227-732463823ed3")
    .buildRequest()
    .patch(printTask);

```