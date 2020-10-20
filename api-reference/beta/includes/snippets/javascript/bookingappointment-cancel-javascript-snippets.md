---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26a22f36d51a70d8c76afe09ec088f914a41a992
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  cancellationMessage: "Your appointment has been successfully cancelled. Please call us again."
};

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel')
    .version('beta')
    .post(cancel);

```