---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee0018966df8fb03deb475ef9c9aaa012417a7b1
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scheduleInformation = {
    schedules: ["adelev@contoso.onmicrosoft.com", "meganb@contoso.onmicrosoft.com"],
    startTime: {
        dateTime: "2019-03-15T09:00:00",
        timeZone: "Pacific Standard Time"
    },
    endTime: {
        dateTime: "2019-03-15T18:00:00",
        timeZone: "Pacific Standard Time"
    },
    availabilityViewInterval: 60
};

let res = await client.api('/me/calendar/getSchedule')
    .post(scheduleInformation);

```