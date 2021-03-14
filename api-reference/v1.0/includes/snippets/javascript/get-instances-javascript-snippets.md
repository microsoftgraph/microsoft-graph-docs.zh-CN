---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d36f2a24d0e1aecf3c20b7eca64f345d4345a295
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let instances = await client.api('/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end')
    .select('subject,bodyPreview,seriesMasterId,type,recurrence,start,end')
    .get();

```