---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e8475806c69018a2acfc45ed8a746e5dc93f4b85
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876139"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionPage recentPlans = graphClient.me().planner().recentPlans()
    .buildRequest()
    .get();

```