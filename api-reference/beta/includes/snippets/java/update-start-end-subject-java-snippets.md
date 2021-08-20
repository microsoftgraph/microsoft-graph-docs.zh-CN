---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f2b505cfde9fcf0670384567dff94b688ffc86c13f089adbfcb3cb7a06ac6a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164103"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
onlineMeeting.startDateTime = OffsetDateTimeSerializer.deserialize("2020-09-09T21:33:30.8546353+00:00");
onlineMeeting.endDateTime = OffsetDateTimeSerializer.deserialize("2020-09-09T22:03:30.8566356+00:00");
onlineMeeting.subject = "Patch Meeting Subject";

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi")
    .buildRequest()
    .patch(onlineMeeting);

```