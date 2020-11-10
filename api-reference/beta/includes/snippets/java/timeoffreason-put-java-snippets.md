---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f59000a027342ea65939aa8576c0c954460cd7e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981383"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

TimeOffReason timeOffReason = new TimeOffReason();
timeOffReason.displayName = "Vacation";
timeOffReason.iconType = TimeOffReasonIconType.PLANE;
timeOffReason.isActive = true;

graphClient.teams("{teamId}").schedule().timeOffReasons("{timeOffReasonId}")
    .buildRequest( requestOptions )
    .put(timeOffReason);

```