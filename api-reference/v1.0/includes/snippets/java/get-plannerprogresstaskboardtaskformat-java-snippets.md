---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9dace798f9494e98a041f227d92841fc00aba4ed
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887075"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").progressTaskBoardFormat()
    .buildRequest()
    .get();

```