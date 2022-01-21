---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45c904465129929c0ac9917283a406e8201d2d09
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  cancellationMessage: 'Your appointment has been successfully cancelled. Please call us again.'
};

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel')
    .version('beta')
    .post(cancel);

```