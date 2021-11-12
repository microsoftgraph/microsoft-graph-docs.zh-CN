---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 606cb7461141a45fb55d41c91aed644d4b677e5895a8dc14c23f42325a35c078
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328859"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionPage plans = graphClient.me().planner().plans()
    .buildRequest()
    .get();

```