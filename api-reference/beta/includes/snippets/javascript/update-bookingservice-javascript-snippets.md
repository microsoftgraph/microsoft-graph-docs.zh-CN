---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9de96554ebb8a31bd38adf77b8967178e573610a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636576"
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
    .update(bookingService);

```