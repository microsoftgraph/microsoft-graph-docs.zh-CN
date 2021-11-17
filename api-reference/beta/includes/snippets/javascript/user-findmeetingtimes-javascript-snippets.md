---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e19223e26a6bd3682ff0c785f7315110aad2849e00ca72bf85b94a0554633ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219835"
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
    isRequired: 'false',  
    suggestLocation: 'false',  
    locations: [ 
      { 
        resolveAvailability: 'false',
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
    .version('beta')
    .post(meetingTimeSuggestionsResult);

```