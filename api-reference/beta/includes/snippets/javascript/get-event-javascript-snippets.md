---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b15db0568e2cc29a6a4c7d0b5302c0ca099a9087d3a3415e5d8e524ffb52e363
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904053"
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