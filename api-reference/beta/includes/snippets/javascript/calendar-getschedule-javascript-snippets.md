---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8b4acacb342533aa7a57182ca8d5a619fc99d4dc043e14eb0142da057fd096c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161897"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scheduleInformation = {
    schedules: ['adelev@contoso.onmicrosoft.com', 'meganb@contoso.onmicrosoft.com'],
    startTime: {
        dateTime: '2019-03-15T09:00:00',
        timeZone: 'Pacific Standard Time'
    },
    endTime: {
        dateTime: '2019-03-15T18:00:00',
        timeZone: 'Pacific Standard Time'
    },
    availabilityViewInterval: 60
};

await client.api('/me/calendar/getSchedule')
    .version('beta')
    .post(scheduleInformation);

```