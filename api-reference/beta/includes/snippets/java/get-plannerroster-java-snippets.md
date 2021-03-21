---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c276bf4c19472aae60ec2dbd53d0c88c12225645
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980840"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRoster plannerRoster = graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965")
    .buildRequest()
    .get();

```