---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa1afeb719bc3d5d62a50510f2bcef49385e70e585638a8b77e6554287acbc4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903952"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucket plannerBucket = graphClient.planner().buckets("hsOf2dhOJkqyYYZEtdzDe2QAIUCR")
    .buildRequest()
    .get();

```