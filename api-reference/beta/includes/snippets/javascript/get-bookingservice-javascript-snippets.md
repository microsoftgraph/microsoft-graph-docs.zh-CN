---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2bea3801691b36fefdbff195273ea426a3cc61d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingService = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976')
    .version('beta')
    .get();

```