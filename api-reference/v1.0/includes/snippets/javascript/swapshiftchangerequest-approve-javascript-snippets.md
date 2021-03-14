---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18de047bf4f1890a5f80fe0f2eb88f04f489d8ea
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve')
    .post(approve);

```