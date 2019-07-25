---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c2eef52d320275af92b1baa07f89b5c3c5aa21f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856925"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting OnlineMeeting = new OnlineMeeting();
OnlineMeeting.meetingType = MeetingType.MEET_NOW;
MeetingParticipants participants = new MeetingParticipants();
MeetingParticipantInfo organizer = new MeetingParticipantInfo();
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "550fae72-d251-43ec-868c-373732c2704f";
identity.user = user;
organizer.identity = identity;
participants.organizer = organizer;
OnlineMeeting.participants = participants;
OnlineMeeting.subject = "subject-value";

graphClient.app().onlineMeetings()
    .buildRequest()
    .post(OnlineMeeting);

```