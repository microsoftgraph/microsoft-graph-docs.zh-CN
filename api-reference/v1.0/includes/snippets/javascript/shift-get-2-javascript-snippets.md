---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c15ee5db8d0b04c08232b541dd638d34a2b5d0e41d37be5357aee0fc5a77fb7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333348"
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