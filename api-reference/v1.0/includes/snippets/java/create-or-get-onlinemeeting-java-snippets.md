---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a38c2b87daf87e06057e6db458bbf678a6bd8f5
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946035"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar startDateTime = CalendarSerializer.deserialize("02/06/2020 01:49:21");

Calendar endDateTime = CalendarSerializer.deserialize("02/06/2020 02:19:21");

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
attendees.upn = "test1@contoso.com";
attendeesList.add(attendees);
participants.attendees = attendeesList;

graphClient.me().onlineMeetings()
    .createOrGet(null,endDateTime,externalId,participants,startDateTime,subject)
    .buildRequest()
    .post();

```