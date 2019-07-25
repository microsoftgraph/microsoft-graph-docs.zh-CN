---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 14e127e0cb069199bfd409ff66280673f7238bcd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892129"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucket plannerBucket = graphClient.planner().buckets("{bucket-id}")
    .buildRequest()
    .get();

```