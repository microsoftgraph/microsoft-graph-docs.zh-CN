---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d7d1521b1fa1ddca3d8a5673b05efa522fc485f51ac341ace884880078886cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334044"
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