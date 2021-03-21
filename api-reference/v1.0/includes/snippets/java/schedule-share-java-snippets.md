---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9723e6d4594ee80490c267029f3a1bf5872909b4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966654"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean notifyTeam = true;

OffsetDateTime startDateTime = OffsetDateTimeSerializer.deserialize("10/08/2018 00:00:00");

OffsetDateTime endDateTime = OffsetDateTimeSerializer.deserialize("10/15/2018 00:00:00");

graphClient.teams("{teamId}").schedule()
    .share(ScheduleShareParameterSet
        .newBuilder()
        .withNotifyTeam(notifyTeam)
        .withStartDateTime(startDateTime)
        .withEndDateTime(endDateTime)
        .build())
    .buildRequest()
    .post();

```