---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 277c1c2d31bfbab2d76f2f47be2f6e8355d40dc9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRoster plannerRoster = new PlannerRoster();

graphClient.planner().rosters()
    .buildRequest()
    .post(plannerRoster);

```