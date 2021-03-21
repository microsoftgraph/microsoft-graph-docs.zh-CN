---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea04f73b2e61b54ca30f91d1f17c42a86a583950
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerAssignedToTaskBoardTaskFormat plannerAssignedToTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").assignedToTaskBoardFormat()
    .buildRequest()
    .get();

```