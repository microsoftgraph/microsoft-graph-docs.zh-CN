---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc03346b15e3bfcf77d636409bbf05fada3eb048
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933795"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
onlineMeeting.meetingType = MeetingType.MEET_NOW;
MeetingParticipants participants = new MeetingParticipants();
MeetingParticipantInfo organizer = new MeetingParticipantInfo();
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "550fae72-d251-43ec-868c-373732c2704f";
identity.user = user;
organizer.identity = identity;
participants.organizer = organizer;
onlineMeeting.participants = participants;
onlineMeeting.subject = "subject-value";

graphClient.app().onlineMeetings()
    .buildRequest()
    .post(onlineMeeting);

```