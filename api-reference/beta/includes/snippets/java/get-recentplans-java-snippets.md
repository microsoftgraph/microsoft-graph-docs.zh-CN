---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ff7dd74ef7e026b05a4d343b2d66776a346ce34
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980480"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionWithReferencesPage recentPlans = graphClient.me().planner().recentPlans()
    .buildRequest()
    .get();

```