---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbc1d8c01e5daca9bf934143263e51b3afe9d92bb554eb0ab8925c603a73ebc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328757"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRosterMember plannerRosterMember = new PlannerRosterMember();
plannerRosterMember.userId = "String";

graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965").members()
    .buildRequest()
    .post(plannerRosterMember);

```