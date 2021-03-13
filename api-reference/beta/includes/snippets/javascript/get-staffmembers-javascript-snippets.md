---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dc6897cfe96c44c7346095bb95c963c3fd20866
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778457"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let staffMembers = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers')
    .version('beta')
    .get();

```