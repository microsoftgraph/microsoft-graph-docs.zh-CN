---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 618d2df2cf174aaad71f8731bc6479c0b76cb2d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingStaffMember = {
    '@odata.type':'#microsoft.graph.bookingStaffMember',
    colorIndex: 1,
    displayName: 'Dana Swope',
    emailAddress: 'danas@contoso.com',
    'role@odata.type':'#microsoft.graph.bookingStaffRole',
    role: 'externalGuest',
    useBusinessHours: true,
    'workingHours@odata.type':'#Collection(microsoft.graph.bookingWorkHours)',
    workingHours: [
        {
            '@odata.type':'#microsoft.graph.bookingWorkHours',
            'day@odata.type':'#microsoft.graph.dayOfWeek',
            day: 'monday',
            'timeSlots@odata.type':'#Collection(microsoft.graph.bookingWorkTimeSlot)',
            timeSlots: [
                {
                    '@odata.type':'#microsoft.graph.bookingWorkTimeSlot',
                    end: '17:00:00.0000000',
                    start: '08:00:00.0000000'
                }
            ]
        },
        {
            '@odata.type':'#microsoft.graph.bookingWorkHours',
            'day@odata.type':'#microsoft.graph.dayOfWeek',
            day: 'tuesday',
            'timeSlots@odata.type':'#Collection(microsoft.graph.bookingWorkTimeSlot)',
            timeSlots: [
                {
                    '@odata.type':'#microsoft.graph.bookingWorkTimeSlot',
                    end: '17:00:00.0000000',
                    start: '08:00:00.0000000'
                }
            ]
        },
        {
            '@odata.type':'#microsoft.graph.bookingWorkHours',
            'day@odata.type':'#microsoft.graph.dayOfWeek',
            day: 'wednesday',
            'timeSlots@odata.type':'#Collection(microsoft.graph.bookingWorkTimeSlot)',
            timeSlots: [
                {
                    '@odata.type':'#microsoft.graph.bookingWorkTimeSlot',
                    end: '17:00:00.0000000',
                    start: '08:00:00.0000000'
                }
            ]
        },
        {
            '@odata.type':'#microsoft.graph.bookingWorkHours',
            'day@odata.type':'#microsoft.graph.dayOfWeek',
            day: 'thursday',
            'timeSlots@odata.type':'#Collection(microsoft.graph.bookingWorkTimeSlot)',
            timeSlots: [
                {
                    '@odata.type':'#microsoft.graph.bookingWorkTimeSlot',
                    end: '17:00:00.0000000',
                    start: '08:00:00.0000000'
                }
            ]
        },
        {
            '@odata.type':'#microsoft.graph.bookingWorkHours',
            'day@odata.type':'#microsoft.graph.dayOfWeek',
            day: 'friday',
            'timeSlots@odata.type':'#Collection(microsoft.graph.bookingWorkTimeSlot)',
            timeSlots: [
                {
                    '@odata.type':'#microsoft.graph.bookingWorkTimeSlot',
                    end: '17:00:00.0000000',
                    start: '08:00:00.0000000'
                }
            ]
        }
    ]
};

await client.api('/bookingBusinesses/{id}/staffMembers')
    .version('beta')
    .post(bookingStaffMember);

```