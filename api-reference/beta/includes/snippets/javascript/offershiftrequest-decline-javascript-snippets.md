---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfad483304b98789a5e2d3369cc7dc6569f0a82c
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: "Sorry, you can't offer this shift."
};

let res = await client.api('/teams/schedule/offerShiftRequests/decline')
    .version('beta')
    .post(decline);

```