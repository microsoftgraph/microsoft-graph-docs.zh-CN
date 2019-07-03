---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fe49276461eb2575eed96cfbeaea9b416f8bccd9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingStaffMember = {
    @odata.type:"#microsoft.graph.bookingStaffMember",
    colorIndex:1,
    displayName:"Dana Swope",
    emailAddress:"danas@contoso.com",
    role@odata.type:"#microsoft.graph.bookingStaffRole",
    role:"externalGuest",
    useBusinessHours:true,
    workingHours@odata.type:"#Collection(microsoft.graph.bookingWorkHours)",
    workingHours:[
        {
            @odata.type:"#microsoft.graph.bookingWorkHours",
            day@odata.type:"#microsoft.graph.dayOfWeek",
            day:"monday",
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

let res = await client.api('/bookingBusinesses/{id}/staffMembers')
    .version('beta')
    .post({bookingStaffMember : bookingStaffMember});

```