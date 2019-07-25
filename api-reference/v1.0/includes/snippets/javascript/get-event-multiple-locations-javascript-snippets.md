---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 47656df44abb3c939c52e5533a7c579b77bc199d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732546"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkADAGAADDdm4NAAA=')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,locations')
    .get();

```