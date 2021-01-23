---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 936d089565b1a548a92371eca3c5c7b2b0cfe813
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945756"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean notifyTeam = true;

Calendar startDateTime = CalendarSerializer.deserialize("10/08/2018 00:00:00");

Calendar endDateTime = CalendarSerializer.deserialize("10/15/2018 00:00:00");

graphClient.teams("{teamId}").schedule()
    .share(notifyTeam,startDateTime,endDateTime)
    .buildRequest()
    .post();

```