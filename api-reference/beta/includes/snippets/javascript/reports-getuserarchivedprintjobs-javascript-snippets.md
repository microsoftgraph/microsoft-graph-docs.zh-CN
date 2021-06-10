---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 158e970b842f80f35927132c645845365de62e27
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getUserArchivedPrintJobs = await client.api('/print/reports/getUserArchivedPrintJobs(userId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)')
    .version('beta')
    .get();

```