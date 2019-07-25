---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fad35cd5433feb9eaedc2aff39a6772103447bad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888762"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskDetails plannerTaskDetails = graphClient.planner().tasks("{task-id}").details()
    .buildRequest()
    .get();

```