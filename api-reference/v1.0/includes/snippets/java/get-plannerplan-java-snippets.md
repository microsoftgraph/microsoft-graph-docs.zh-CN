---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb69d1b47cd57830d118a0459bfad901b52199ede01427148538f3bd37048fec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104303"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = graphClient.planner().plans("{plan-id}")
    .buildRequest()
    .get();

```