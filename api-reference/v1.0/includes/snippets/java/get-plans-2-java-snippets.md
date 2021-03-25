---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63be497cf482463488b9eec410a3f4c59c0aad78
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208734"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionPage plans = graphClient.groups("{group-id}").planner().plans()
    .buildRequest()
    .get();

```