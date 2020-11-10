---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 519171b472706ed0eb0ba860b17e9bb98b6300e0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980141"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatInfo chatInfo = new ChatInfo();
chatInfo.threadId = "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2";

Calendar startDateTime = CalendarSerializer.deserialize("2/6/2020 1:49:21 AM");

Calendar endDateTime = CalendarSerializer.deserialize("2/6/2020 2:19:21 AM");

String externalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56";

MeetingParticipants participants = new MeetingParticipants();
LinkedList<MeetingParticipantInfo> attendeesList = new LinkedList<MeetingParticipantInfo>();
MeetingParticipantInfo attendees = new MeetingParticipantInfo();
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "1f35f2e6-9cab-44ad-8d5a-b74c14720000";
identity.user = user;
attendees.identity = identity;
attendees.upn = "test1@contoso.com";
attendeesList.add(attendees);
participants.attendees = attendeesList;

String subject = "Create a meeting with customId provided";

graphClient.me().onlineMeetings()
    .createOrGet(chatInfo,endDateTime,externalId,participants,startDateTime,subject)
    .buildRequest()
    .post();

```