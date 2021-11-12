---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e55eeba5b4dd5c61c79b52796ca80d932bc02cc2d5b732738a7d1a71877cea10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getPrinterArchivedPrintJobs = await client.api('/print/reports/getPrinterArchivedPrintJobs(printerId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)')
    .version('beta')
    .get();

```