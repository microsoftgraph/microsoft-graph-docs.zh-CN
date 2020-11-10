---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e943203e4f46b7ed3a91c99bbad001cfbf9a644e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978226"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = graphClient.planner().plans("{id}")
    .buildRequest()
    .get();

```