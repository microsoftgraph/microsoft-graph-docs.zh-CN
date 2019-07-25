---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a2d0e7b7ae18ccf7ff58c9a20c430978bacc89ba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870938"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISchedulingGroupCollectionPage schedulingGroups = graphClient.teams("{teamId}").schedule().schedulingGroups()
    .buildRequest()
    .get();

```