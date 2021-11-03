---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0002a28704bb64a4fee2aa324a821db549af74f9ecc102895b9f13ef054b852e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162301"
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

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976')
    .version('beta')
    .update(bookingService);

```