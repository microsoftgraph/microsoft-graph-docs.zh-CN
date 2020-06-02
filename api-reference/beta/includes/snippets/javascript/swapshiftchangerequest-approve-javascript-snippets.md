---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15cda19c2a35cfc2609081601fadb19238e9e528
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219211"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: "message-value"
};

let res = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve')
    .version('beta')
    .post(approve);

```