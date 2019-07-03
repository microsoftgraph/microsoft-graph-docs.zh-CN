---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d05366f4e69a696f31acf0d1ea54b5ba6a068bb9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480161"
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