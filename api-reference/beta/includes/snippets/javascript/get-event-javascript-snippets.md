---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8452d9a1ae2b1b680e2942169fad3ae0ea41b888
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkAGIAAAoZDOFAAA=/')
    .version('beta')
    .header('Prefer','outlook.timezone="Pacific Standard Time"')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees')
    .get();

```