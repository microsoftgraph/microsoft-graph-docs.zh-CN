---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffc57f29c9899f24123fc609bbae5e7155866756
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216387"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean notifyTeam = true;

int startDateTime = 10/8/2018 12:00:00 AM;

int endDateTime = 10/15/2018 12:00:00 AM;

graphClient.teams("{teamId}").schedule()
    .share(notifyTeam,startDateTime,endDateTime)
    .buildRequest()
    .post();

```