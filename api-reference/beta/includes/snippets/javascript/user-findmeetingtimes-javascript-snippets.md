---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 688f49c97a6cdc4db361e293a6b32171ab5cfbbe
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44533568"
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
    .version('beta')
    .post(meetingTimeSuggestionsResult);

```