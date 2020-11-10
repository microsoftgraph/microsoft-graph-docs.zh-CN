---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2d0e7b7ae18ccf7ff58c9a20c430978bacc89ba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969854"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISchedulingGroupCollectionPage schedulingGroups = graphClient.teams("{teamId}").schedule().schedulingGroups()
    .buildRequest()
    .get();

```