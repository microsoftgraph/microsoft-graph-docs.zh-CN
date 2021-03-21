---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbf9d9792aa16e353ba29eff42d9c759f0f3568f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const shiftPreferences = {
    id: 'SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7',
    '@odata.etag': '1a371e53-f0a6-4327-a1ee-e3c56e4b38aa',
    availability: [
        {
            recurrence: {
                pattern: {
                    type: 'Weekly',
                    daysOfWeek: ['Monday', 'Wednesday', 'Friday'],
                    interval: 1
                },
                range: {
                    type: 'noEnd'
                }
            },
            timeZone: 'Pacific Standard Time',
            timeSlots: null
        }
    ]
};

await client.api('/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences')
    .update(shiftPreferences);

```