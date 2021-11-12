---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3c11f4cb0e78385fa9cc9ee2af28cbdeb334426f2e4ab210bb4e0ff81866cfd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903668"
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