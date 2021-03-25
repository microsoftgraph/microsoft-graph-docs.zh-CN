---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4340be12c01b64b527629dac2d72255181af50d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210327"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatInfo chatInfo = new ChatInfo();
chatInfo.threadId = "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2";

OffsetDateTime startDateTime = OffsetDateTimeSerializer.deserialize("02/06/2020 01:49:21");

OffsetDateTime endDateTime = OffsetDateTimeSerializer.deserialize("02/06/2020 02:19:21");

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
    .createOrGet(OnlineMeetingCreateOrGetParameterSet
        .newBuilder()
        .withChatInfo(chatInfo)
        .withEndDateTime(endDateTime)
        .withExternalId(externalId)
        .withParticipants(participants)
        .withStartDateTime(startDateTime)
        .withSubject(subject)
        .build())
    .buildRequest()
    .post();

```