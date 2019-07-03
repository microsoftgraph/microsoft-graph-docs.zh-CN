---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a8262be592fc3cdf9ba98bbe5ce5e483319bdbbd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingService = {
    @odata.type:"#microsoft.graph.bookingService",
    defaultDuration:"PT30M"
};

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976')
    .version('beta')
    .update({bookingService : bookingService});

```