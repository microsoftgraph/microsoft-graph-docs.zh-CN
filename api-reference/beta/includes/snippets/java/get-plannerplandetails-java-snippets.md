---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef842bf4f3a0a0cc15ad12b09df7fdded0d8faf9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982404"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanDetails plannerPlanDetails = graphClient.planner().plans("xqQg5FS2LkCp935s-FIFm2QAFkHM").details()
    .buildRequest()
    .get();

```