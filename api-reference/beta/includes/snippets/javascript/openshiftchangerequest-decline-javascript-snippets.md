---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fb5a41e729e7ddfe7cf8d518da56f4e73860c08
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795944"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: 'message-value'
};

await client.api('/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline')
    .version('beta')
    .post(decline);

```