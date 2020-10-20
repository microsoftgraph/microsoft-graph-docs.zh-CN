---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d05366f4e69a696f31acf0d1ea54b5ba6a068bb9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end')
    .version('beta')
    .select('subject,bodyPreview,seriesMasterId,type,recurrence,start,end')
    .get();

```