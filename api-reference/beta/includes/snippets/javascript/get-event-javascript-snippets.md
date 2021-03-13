---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfd54a99e4fe6a168d0ccc0fa0570e10543c0645
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/me/events/AAMkAGIAAAoZDOFAAA=/')
    .version('beta')
    .header('Prefer','outlook.timezone="Pacific Standard Time"')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees')
    .get();

```