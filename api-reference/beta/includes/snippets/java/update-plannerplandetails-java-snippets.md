---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b8da94fb28dfd08f5e764d17a6ff047f3dbf303
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977078"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
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

graphClient.planner().plans("xqQg5FS2LkCp935s-FIFm2QAFkHM").details()
    .buildRequest( requestOptions )
    .patch(plannerPlanDetails);

```