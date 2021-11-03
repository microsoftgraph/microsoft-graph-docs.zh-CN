---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4857805febc6cc481d1c06829d8c81eab7761484d9c57c2d0c87f1eaa3cb01e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903134"
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