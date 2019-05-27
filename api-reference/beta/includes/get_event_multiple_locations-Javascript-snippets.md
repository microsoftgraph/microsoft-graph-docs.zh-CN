---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 02da2f480bc33ca2d0bc66f35ebfd5ee06a924d8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkADAGAADDdm4NAAA=/')
    .version('beta')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,locations')
    .get();

```