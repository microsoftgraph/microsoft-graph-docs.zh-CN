---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2d78132e46fe89b7738262544d5ea2558e760186e623dc56a8e641f1b6f740a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163928"
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