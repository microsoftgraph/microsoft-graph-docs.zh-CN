---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 531a47e9f0a9fee612cb931e328d55272a5ea301
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48907257"
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
    isRequired: false,  
    suggestLocation: false,  
    locations: [ 
      { 
        resolveAvailability: false,
        displayName: "Conf room Hood" 
      } 
    ] 
  },  
  timeConstraint: {
    activityDomain:"work", 
    timeSlots: [ 
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