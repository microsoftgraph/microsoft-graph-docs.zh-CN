---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dd08c79823466813907409f6f96436d31fe1f031523fecb8b524c1d3df7c80a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903861"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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