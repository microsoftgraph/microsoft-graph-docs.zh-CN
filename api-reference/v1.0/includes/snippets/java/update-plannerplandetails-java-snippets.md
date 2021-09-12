---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5af5c71989c681ef7d632b7970476eb47fc1e6882c1a10c7e6eda44eee0a127
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904299"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerPlanDetails plannerPlanDetails = new PlannerPlanDetails();
PlannerUserIds sharedWith = new PlannerUserIds();
sharedWith.6463a5ce-2119-4198-9f2a-628761df4a62 = true;
sharedWith.d95e6152-f683-4d78-9ff5-67ad180fea4a = false;
plannerPlanDetails.sharedWith = sharedWith;
PlannerCategoryDescriptions categoryDescriptions = new PlannerCategoryDescriptions();
categoryDescriptions.category1 = "Indoors";
categoryDescriptions.category3 = null;
plannerPlanDetails.categoryDescriptions = categoryDescriptions;

graphClient.planner().plans("{plan-id}").details()
    .buildRequest( requestOptions )
    .patch(plannerPlanDetails);

```