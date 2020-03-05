---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae8b2f98c29e6ca17e7f1efb36a9d9e91ab18244
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: "message-value"
};

let res = await client.api('/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve')
    .version('beta')
    .post(approve);

```