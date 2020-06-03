---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f7fad3ed8377ec4dd3897dac7a2aeaa6e253e65
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215911"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: "message-value"
};

let res = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline')
    .post(decline);

```