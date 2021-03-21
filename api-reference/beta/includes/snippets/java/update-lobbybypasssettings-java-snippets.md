---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d22a7533a8caa5aa958b195d728bd8f70e68d8cd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
LobbyBypassSettings lobbyBypassSettings = new LobbyBypassSettings();
lobbyBypassSettings.isDialInBypassEnabled = true;
onlineMeeting.lobbyBypassSettings = lobbyBypassSettings;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi")
    .buildRequest()
    .patch(onlineMeeting);

```