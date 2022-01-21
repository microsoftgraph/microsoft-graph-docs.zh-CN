---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fc88eb5d069eb9b24e982257b0042b865ebc22f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6')
    .version('beta')
    .delete();

```