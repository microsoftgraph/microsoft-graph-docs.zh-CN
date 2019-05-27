---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a8262be592fc3cdf9ba98bbe5ce5e483319bdbbd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465543"
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