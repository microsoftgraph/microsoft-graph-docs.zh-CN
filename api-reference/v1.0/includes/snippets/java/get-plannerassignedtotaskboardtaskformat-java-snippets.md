---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43f1e1e0dce746c763523a37add1c8c3adc9a65d223d0c1dd1cd52222dc489ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831185"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerAssignedToTaskBoardTaskFormat plannerAssignedToTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").assignedToTaskBoardFormat()
    .buildRequest()
    .get();

```