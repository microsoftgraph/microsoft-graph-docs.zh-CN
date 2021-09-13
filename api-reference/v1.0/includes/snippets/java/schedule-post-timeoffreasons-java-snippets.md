---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f743bb0445a69a9c4987cb702ebaa54cc6c325f936aa7a2455da9837baedbf3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277857"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffReason timeOffReason = new TimeOffReason();
timeOffReason.displayName = "Vacation";
timeOffReason.iconType = TimeOffReasonIconType.PLANE;
timeOffReason.isActive = true;

graphClient.teams("{teamId}").schedule().timeOffReasons()
    .buildRequest()
    .post(timeOffReason);

```