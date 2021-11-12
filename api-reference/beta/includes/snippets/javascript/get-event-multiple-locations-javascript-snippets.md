---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6b2032e37d9f78cdd6a125e8214c177c7b550f9a81c0d0415945cbcb435d603
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/me/events/AAMkADAGAADDdm4NAAA=/')
    .version('beta')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,locations')
    .get();

```