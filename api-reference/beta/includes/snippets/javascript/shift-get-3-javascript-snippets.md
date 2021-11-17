---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88c2bcdaafb191f756eb037245a8583e7c7e931e771e590d5adce982afb5dcf4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104702"
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
    .version('beta')
    .put(shiftPreferences);

```