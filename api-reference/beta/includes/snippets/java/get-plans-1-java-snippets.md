---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20efb7c96b4fb59fdd2b5360d777453b6a404580
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210629"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionPage plans = graphClient.planner().plans()
    .buildRequest()
    .get();

```