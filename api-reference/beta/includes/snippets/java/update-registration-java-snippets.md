---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17f66410fee92913c3785c0c927cc082979f35da
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561023"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistration meetingRegistration = new MeetingRegistration();
meetingRegistration.subject = "Microsoft Ignite: Day 1";
meetingRegistration.startDateTime = OffsetDateTimeSerializer.deserialize("2021-11-02T16:00:00+00:00");
meetingRegistration.endDateTime = OffsetDateTimeSerializer.deserialize("2021-11-02T23:45:00+00:00");
LinkedList<MeetingSpeaker> speakersList = new LinkedList<MeetingSpeaker>();
MeetingSpeaker speakers = new MeetingSpeaker();
speakers.displayName = "Henry Ross";
speakers.bio = "Chairman and Chief Executive Officer";
speakersList.add(speakers);
MeetingSpeaker speakers1 = new MeetingSpeaker();
speakers1.displayName = "Fred Ryan";
speakers1.bio = "CVP";
speakersList.add(speakers1);
meetingRegistration.speakers = speakersList;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration()
    .buildRequest()
    .patch(meetingRegistration);

```