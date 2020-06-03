---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a6e39fae6a02b3c67303882ea5fd27d10fd1d4d
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const shiftPreferences = {
    id: "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    @odata.etag: "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    availability: [
        {
            recurrence: {
                pattern: {
                    type: "Weekly",
                    daysOfWeek: ["Monday", "Wednesday", "Friday"],
                    interval: 1
                },
                range: {
                    type: "noEnd"
                }
            },
            timeZone: "Pacific Standard Time",
            timeSlots: null
        }
    ]
};

let res = await client.api('/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences')
    .put(shiftPreferences);

```