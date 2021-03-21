---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3385e21c24ad94421cc768a6ed2683b1f468e801
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974689"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTask printTask = new PrintTask();
PrintTaskStatus status = new PrintTaskStatus();
status.state = PrintTaskProcessingState.COMPLETED;
status.description = "completed";
printTask.status = status;

graphClient.print().taskDefinitions("{taskDefinitionId}").tasks("{taskId}")
    .buildRequest()
    .patch(printTask);

```