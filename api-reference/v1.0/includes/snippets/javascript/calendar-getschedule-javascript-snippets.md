---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df4b7b024f1659da44295eb2e93ece707f07dd52fd31768665582bfe53d8f186
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331851"
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
    .post(scheduleInformation);

```