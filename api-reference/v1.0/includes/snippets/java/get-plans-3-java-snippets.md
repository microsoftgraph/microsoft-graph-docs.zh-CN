---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82326bc31d0ad7bec24094e4ec96ba3cbe4539ad
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210596"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionPage plans = graphClient.me().planner().plans()
    .buildRequest()
    .get();

```