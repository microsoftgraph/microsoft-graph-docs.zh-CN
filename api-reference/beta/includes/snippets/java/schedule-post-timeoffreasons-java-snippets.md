---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb3ad5d4ecd8817cc3467ff7b2826b30909387e4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974950"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffReason timeOffReason = new TimeOffReason();
timeOffReason.displayName = "Vacation";
timeOffReason.iconType = TimeOffReasonIconType.PLANE;
timeOffReason.isActive = true;

graphClient.teams("{teamId}").schedule().timeOffReasons()
    .buildRequest()
    .post(timeOffReason);

```