---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65bbd9a9fb8f8d9330c303468bd3cc2df685316b
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217633"
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
    .post(decline);

```