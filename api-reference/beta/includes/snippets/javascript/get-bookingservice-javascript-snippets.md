---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bfdd231fa12fe8a612b0f048ead43f6c35c4797
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805086"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingService = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976')
    .version('beta')
    .get();

```