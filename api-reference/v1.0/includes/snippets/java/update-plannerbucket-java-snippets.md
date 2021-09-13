---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb474bbbe002bb44c76ccc5957fe9b49e90c62f00f4e02adaaaba827f43e53b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218706"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerBucket plannerBucket = new PlannerBucket();
plannerBucket.name = "Development";

graphClient.planner().buckets("{bucket-id}")
    .buildRequest( requestOptions )
    .patch(plannerBucket);

```