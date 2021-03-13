---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6db41305a75a7dc8a48201f259b56286fb05771
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791464"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingStaffMember = {
    workingHours: [
        {
            '@odata.type':'#microsoft.graph.bookingWorkHours',
            'day@odata.type':'#microsoft.graph.dayOfWeek',
            day: 'monday',
            'timeSlots@odata.type':'#Collection(microsoft.graph.bookingWorkTimeSlot)',
            timeSlots: [

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

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148')
    .version('beta')
    .update(bookingStaffMember);

```