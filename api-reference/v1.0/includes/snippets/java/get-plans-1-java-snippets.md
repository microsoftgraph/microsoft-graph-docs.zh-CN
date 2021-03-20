---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99068aa09f512553957ecdb80bdd6e725c279e9e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941510"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionPage plans = graphClient.planner().plans()
    .buildRequest()
    .get();

```