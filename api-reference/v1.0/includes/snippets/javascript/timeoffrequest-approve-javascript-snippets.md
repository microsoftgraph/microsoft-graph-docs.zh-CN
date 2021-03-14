---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b584f26e3ee9cd69563a5143ce2d1ef69c3b7ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve')
    .post(approve);

```