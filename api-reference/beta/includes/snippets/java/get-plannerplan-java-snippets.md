---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f547bb10e728dee4c28b97edcb0825cd1a80e0f7aaf594325a42386ddee6cc13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161393"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = graphClient.planner().plans("{id}")
    .buildRequest()
    .get();

```