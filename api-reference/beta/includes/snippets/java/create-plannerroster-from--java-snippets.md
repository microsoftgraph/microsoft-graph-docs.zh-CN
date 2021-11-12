---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74d09f07aab64a27758f561bf1b9363252250fc5eb533aed79c35af679c12dd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103972"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRoster plannerRoster = new PlannerRoster();

graphClient.planner().rosters()
    .buildRequest()
    .post(plannerRoster);

```