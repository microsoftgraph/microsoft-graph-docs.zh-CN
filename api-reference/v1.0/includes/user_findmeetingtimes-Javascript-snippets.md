---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5968e6c787d47e179ea3a8482eb7fc87bbcd52de
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingTimeSuggestionsResult = {
  attendees: [ 
    { 
      type: "required",  
      emailAddress: { 
        name: "Alex Wilbur",
        address: "alexw@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  locationConstraint: { 
    isRequired: "false",  
    suggestLocation: "false",  
    locations: [ 
      { 
        resolveAvailability: "false",
        displayName: "Conf room Hood" 
      } 
    ] 
  },  
  timeConstraint: {
    activityDomain:"work", 
    timeslots: [ 
      { 
        start: { 
          dateTime: "2019-04-16T09:00:00",  
          timeZone: "Pacific Standard Time" 
        },  
        end: { 
          dateTime: "2019-04-18T17:00:00",  
          timeZone: "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  isOrganizerOptional: "false",
  meetingDuration: "PT1H",
  returnSuggestionReasons: "true",
  minimumAttendeePercentage: "100"
};

let res = await client.api('/me/findMeetingTimes')
    .post(meetingTimeSuggestionsResult);

```