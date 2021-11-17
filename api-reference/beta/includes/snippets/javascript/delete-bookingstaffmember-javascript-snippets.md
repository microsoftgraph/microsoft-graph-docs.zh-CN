---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae3bc37ff205a1a17689c2194f279bef9e8ab7ef823ca1d9db27778f2cf280cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6')
    .version('beta')
    .delete();

```