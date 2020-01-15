---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3ac39416172a377d697d8cfcf79022fb3d630a2
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00')
    .get();

```