---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b560dda95db0ae6e207d6cea61b4a9e65dc20e91
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getGroupArchivedPrintJobs = await client.api('/print/reports/getGroupArchivedPrintJobs(groupId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)')
    .version('beta')
    .get();

```