---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49378d46e6b869a74ceda123bc4301fe023838db
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44218168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: "Approved!"
};

let res = await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve')
    .post(approve);

```