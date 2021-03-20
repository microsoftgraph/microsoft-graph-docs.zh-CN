---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4a6e48b3421a0aea3eb25b1721183ba24d2f2c6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953220"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionWithReferencesPage rosterPlans = graphClient.users("{usersId}").planner().rosterPlans()
    .buildRequest()
    .get();

```