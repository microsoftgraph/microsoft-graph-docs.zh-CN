---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0779e103a8e35f6689f91c81d7d27c93e5b486a5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478178"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingStaffMember = {
    workingHours:[
        {
            @odata.type:"#microsoft.graph.bookingWorkHours",
            day@odata.type:"#microsoft.graph.dayOfWeek",
            day:"monday",
            timeSlots@odata.type:"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            timeSlots:[

            ]
        },
        {
            @odata.type:"#microsoft.graph.bookingWorkHours",
            day@odata.type:"#microsoft.graph.dayOfWeek",
            day:"tuesday",
            timeSlots@odata.type:"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            timeSlots:[
                {
                    @odata.type:"#microsoft.graph.bookingWorkTimeSlot",
                    end:"17:00:00.0000000",
                    start:"08:00:00.0000000"
                }
            ]
        },
        {
            @odata.type:"#microsoft.graph.bookingWorkHours",
            day@odata.type:"#microsoft.graph.dayOfWeek",
            day:"wednesday",
            timeSlots@odata.type:"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            timeSlots:[
                {
                    @odata.type:"#microsoft.graph.bookingWorkTimeSlot",
                    end:"17:00:00.0000000",
                    start:"08:00:00.0000000"
                }
            ]
        },
        {
            @odata.type:"#microsoft.graph.bookingWorkHours",
            day@odata.type:"#microsoft.graph.dayOfWeek",
            day:"thursday",
            timeSlots@odata.type:"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            timeSlots:[
                {
                    @odata.type:"#microsoft.graph.bookingWorkTimeSlot",
                    end:"17:00:00.0000000",
                    start:"08:00:00.0000000"
                }
            ]
        },
        {
            @odata.type:"#microsoft.graph.bookingWorkHours",
            day@odata.type:"#microsoft.graph.dayOfWeek",
            day:"friday",
            timeSlots@odata.type:"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            timeSlots:[
                {
                    @odata.type:"#microsoft.graph.bookingWorkTimeSlot",
                    end:"17:00:00.0000000",
                    start:"08:00:00.0000000"
                }
            ]
        }
    ]
};

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148')
    .version('beta')
    .update({bookingStaffMember : bookingStaffMember});

```