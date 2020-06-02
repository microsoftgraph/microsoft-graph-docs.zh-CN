---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a0bf6f8a7faf1273e25bf7ce3bdd8f2efb25608
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: "Sorry, you can't offer this shift."
};

let res = await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline')
    .version('beta')
    .post(decline);

```