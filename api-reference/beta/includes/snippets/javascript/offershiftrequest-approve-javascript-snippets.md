---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: faeae83a31daa53ca1bd8589dcb0bd322bc33687
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216597"
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
    .version('beta')
    .post(approve);

```