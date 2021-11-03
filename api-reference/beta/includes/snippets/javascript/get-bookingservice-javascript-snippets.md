---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e93c732ac3a1be3862ebea6fd792747a95517a2061930e59a09be7530360e6a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161758"
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