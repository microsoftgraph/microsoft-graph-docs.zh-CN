---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eb4539449816d960927477ba6f4a446976578d60ce4141edf00f65f0aa78d9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106125"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OffsetDateTime startDateTime = OffsetDateTimeSerializer.deserialize("02/06/2020 01:49:21");

OffsetDateTime endDateTime = OffsetDateTimeSerializer.deserialize("02/06/2020 02:19:21");

String subject = "Create a meeting with customId provided";

String externalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56";

MeetingParticipants participants = new MeetingParticipants();
LinkedList<MeetingParticipantInfo> attendeesList = new LinkedList<MeetingParticipantInfo>();
MeetingParticipantInfo attendees = new MeetingParticipantInfo();
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "1f35f2e6-9cab-44ad-8d5a-b74c14720000";
identity.user = user;
attendees.identity = identity;
attendees.role = OnlineMeetingRole.PRESENTER;
attendees.upn = "test1@contoso.com";
attendeesList.add(attendees);
participants.attendees = attendeesList;

graphClient.me().onlineMeetings()
    .createOrGet(OnlineMeetingCreateOrGetParameterSet
        .newBuilder()
        .withChatInfo(null)
        .withEndDateTime(endDateTime)
        .withExternalId(externalId)
        .withParticipants(participants)
        .withStartDateTime(startDateTime)
        .withSubject(subject)
        .build())
    .buildRequest()
    .post();

```