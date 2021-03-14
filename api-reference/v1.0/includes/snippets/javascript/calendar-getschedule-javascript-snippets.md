---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6c636ddff2567f81635b4270467a8bcd59e9965
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780163"
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