---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56a7ee8f4774fd0c9c941981b3d0071b025f83d44c61b5f9f8f2b616068f41a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904095"
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