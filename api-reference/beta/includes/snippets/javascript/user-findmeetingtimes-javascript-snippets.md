---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7d8748a3c9bc6ba05d409fa56e4a05298f7c9791
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500104"
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
    .version('beta')
    .post(meetingTimeSuggestionsResult);

```