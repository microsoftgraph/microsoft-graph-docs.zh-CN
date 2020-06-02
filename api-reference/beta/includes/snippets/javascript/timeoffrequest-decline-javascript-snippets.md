---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7cfe46666024d7affddd2c0b6c0e20836f98638
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217113"
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
    .version('beta')
    .post(decline);

```