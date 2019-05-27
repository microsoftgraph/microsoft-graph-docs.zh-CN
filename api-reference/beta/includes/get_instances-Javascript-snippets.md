---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c461568bb2617e201ffbdc2ec268a3a851848915
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449389"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkAGUzYRgWAAA=/instances')
    .version('beta')
    .select('subject,bodyPreview,seriesMasterId,type,recurrence,start,end')
    .get();

```