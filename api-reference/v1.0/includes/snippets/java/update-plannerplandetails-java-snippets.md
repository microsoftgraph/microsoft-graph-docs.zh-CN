---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37953c148bf28d1a71001401fe3a857a46983069
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573168"
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