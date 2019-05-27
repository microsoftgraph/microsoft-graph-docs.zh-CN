---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31cd939a0755e70a9f589a6b0c499043407b7426
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462990"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkAGUzYRgWAAA=/instances')
    .select('subject,bodyPreview,seriesMasterId,type,recurrence,start,end')
    .get();

```