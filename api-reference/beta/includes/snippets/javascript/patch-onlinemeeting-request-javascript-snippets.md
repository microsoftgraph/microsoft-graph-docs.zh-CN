---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 886b2e6fda7c472eaba26e4fc7a3e2a37560b3f0
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
    startDateTime: "2020-09-09T14:33:30.8546353-07:00", 

    endDateTime: "2020-09-09T15:03:30.8566356-07:00", 

    subject: "Patch Meeting Subject" 
};

let res = await client.api('/me/onlineMeetings/{id}')
    .version('beta')
    .update(onlineMeeting);

```