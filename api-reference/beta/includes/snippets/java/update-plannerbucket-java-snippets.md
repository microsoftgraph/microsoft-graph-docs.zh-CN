---
description: 自动生成的文件。 不修改
ms.openlocfilehash: df0d8b0d2025a51564d990316af03d2de0edd60a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876531"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerBucket plannerBucket = new PlannerBucket();
plannerBucket.name = "Development";

graphClient.planner().buckets("hsOf2dhOJkqyYYZEtdzDe2QAIUCR")
    .buildRequest( requestOptions )
    .patch(plannerBucket);

```