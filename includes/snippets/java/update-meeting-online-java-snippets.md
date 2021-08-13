---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bea0b08054e32cbc16680a6c95277b3d8dd6b094928c04c2c746bb2b3a03a33
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240518"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.isOnlineMeeting = true;
event.onlineMeetingProvider = OnlineMeetingProviderType.TEAMS_FOR_BUSINESS;

graphClient.me().events("AAMkADAGu0AABIGYDaAAA=")
    .buildRequest()
    .patch(event);

```