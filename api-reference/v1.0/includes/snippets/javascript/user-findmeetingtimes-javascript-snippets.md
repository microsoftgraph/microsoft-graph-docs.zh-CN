---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 406f8f25ea9a2ba850dc0c42569a6c47441fcce5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788631"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingTimeSuggestionsResult = {
  attendees: [ 
    { 
      type: 'required',  
      emailAddress: { 
        name: 'Alex Wilbur',
        address: 'alexw@contoso.onmicrosoft.com' 
      } 
    }
  ],  
  locationConstraint: { 
    isRequired: false,  
    suggestLocation: false,  
    locations: [ 
      { 
        resolveAvailability: false,
        displayName: 'Conf room Hood' 
      } 
    ] 
  },  
  timeConstraint: {
    activityDomain: 'work', 
    timeSlots: [ 
      { 
        start: { 
          dateTime: '2019-04-16T09:00:00',  
          timeZone: 'Pacific Standard Time' 
        },  
        end: { 
          dateTime: '2019-04-18T17:00:00',  
          timeZone: 'Pacific Standard Time' 
        } 
      } 
    ] 
  },  
  isOrganizerOptional: 'false',
  meetingDuration: 'PT1H',
  returnSuggestionReasons: 'true',
  minimumAttendeePercentage: '100'
};

await client.api('/me/findMeetingTimes')
    .post(meetingTimeSuggestionsResult);

```