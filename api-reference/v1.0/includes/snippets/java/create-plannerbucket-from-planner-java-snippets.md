---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5709bb98d40f0b696796a69e9807afd949b36ec6
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35856882"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucket plannerBucket = new PlannerBucket();
plannerBucket.name = "Advertising";
plannerBucket.planId = "xqQg5FS2LkCp935s-FIFm2QAFkHM";
plannerBucket.orderHint = " !";

graphClient.planner().buckets()
    .buildRequest()
    .post(plannerBucket);

```