---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40214c5d76099776b27e0fdc5e76e03a14791b19
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/unpublish')
    .version('beta')
    .post();

```