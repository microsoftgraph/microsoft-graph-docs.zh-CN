---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb14932034da3a56d760412290d191d66b3bb088
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219216"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: "message-value"
};

let res = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline')
    .version('beta')
    .post(decline);

```