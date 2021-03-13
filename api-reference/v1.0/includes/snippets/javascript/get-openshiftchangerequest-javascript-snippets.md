---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf07cfc353d9e2e98a57520f62d55c9833bbcd78
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShiftChangeRequest = await client.api('/teams/{id}/schedule/openShiftChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09')
    .get();

```