---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f317f1e1fda2bfd20c7bc920867a262d88864c945168a7164cf12d2c59ca96e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332783"
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