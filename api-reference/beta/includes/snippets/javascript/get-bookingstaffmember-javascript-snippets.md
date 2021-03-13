---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96ed124ea0a011a772252fbb4f86df05a40a8be1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingStaffMember = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51')
    .version('beta')
    .get();

```