---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e02ecb8449a7a28f9b720353f168aca27370855
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957794"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatInfo chatInfo = new ChatInfo();
chatInfo.threadId = "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2";

Calendar startDateTime = CalendarSerializer.deserialize("02/06/2020 01:49:21");

Calendar endDateTime = CalendarSerializer.deserialize("02/06/2020 02:19:21");

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