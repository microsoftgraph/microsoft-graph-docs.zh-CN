---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01d9a704c246ed1b87c7dda786798076666bced3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketCollectionPage buckets = graphClient.planner().buckets()
    .buildRequest()
    .get();

```