---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7b34bea24168df8e8c489d9c335bff57d1e6a1d
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842797"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int startDateTime = 2/6/2020 1:49:21 AM;

int endDateTime = 2/6/2020 2:19:21 AM;

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