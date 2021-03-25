---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f29d567d90c48f3e900878e8c60ba86541502143
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210795"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketCollectionPage buckets = graphClient.planner().plans("{plan-id}").buckets()
    .buildRequest()
    .get();

```