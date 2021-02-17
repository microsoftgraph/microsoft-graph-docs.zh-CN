---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa6635df34c9e7bdecbbf5902ad6676a88c28e39
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272551"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerRosterMemberCollectionPage members = graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965").members()
    .buildRequest()
    .get();

```