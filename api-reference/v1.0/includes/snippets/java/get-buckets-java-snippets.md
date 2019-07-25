---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0d7e91d7fdc0496108c6a29f7b34b22a30120c3f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887130"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerBucketCollectionPage buckets = graphClient.planner().plans("{plan-id}").buckets()
    .buildRequest()
    .get();

```