---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 088b29180924ffebebbed750f780d8001b87f1d5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978388"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerAssignedToTaskBoardTaskFormat plannerAssignedToTaskBoardTaskFormat = graphClient.planner().tasks("01gzSlKkIUSUl6DF_EilrmQAKDhh").assignedToTaskBoardFormat()
    .buildRequest()
    .get();

```