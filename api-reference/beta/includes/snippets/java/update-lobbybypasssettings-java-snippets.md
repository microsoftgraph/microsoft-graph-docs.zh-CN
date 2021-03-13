---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecad7c621f83ef3e0def8d894948ffd6460b5f39
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775631"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
LobbyBypassSettings lobbyBypassSettings = new LobbyBypassSettings();
lobbyBypassSettings.isDialInBypassEnabled = true;
onlineMeeting.lobbyBypassSettings = lobbyBypassSettings;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi")
    .buildRequest()
    .patch(onlineMeeting);

```