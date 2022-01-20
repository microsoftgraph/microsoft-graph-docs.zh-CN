---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 851e6313a0be57154a8cb4ff1e835ac4e8f923ba
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingService = {
    '@odata.type':'#microsoft.graph.bookingService',
    defaultDuration: 'PT30M'
};

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976')
    .version('beta')
    .update(bookingService);

```