---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eab34f2c56cc73bd3f6483eaeaf8e193e149a871
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments')
    .version('beta')
    .get();

```