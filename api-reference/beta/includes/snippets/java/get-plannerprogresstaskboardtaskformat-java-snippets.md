---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8ee1a63573c36e8c19d1c5eed770ffd326f0bcd9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876315"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = graphClient.planner().tasks("'id'").progressTaskBoardFormat()
    .buildRequest()
    .get();

```