---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 660cff2894c693c483d95d4449aa57a69e86284e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/fabrikam@contoso.onmicrosoft.com')
    .version('beta')
    .delete();

```