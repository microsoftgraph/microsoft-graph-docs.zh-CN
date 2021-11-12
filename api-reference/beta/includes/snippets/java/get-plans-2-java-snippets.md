---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6db807396ad4fd32caba79c905c616f7d95a366bc22e1d50eda67f528400b8e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328868"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionPage plans = graphClient.groups("ebf3b108-5234-4e22-b93d-656d7dae5874").planner().plans()
    .buildRequest()
    .get();

```