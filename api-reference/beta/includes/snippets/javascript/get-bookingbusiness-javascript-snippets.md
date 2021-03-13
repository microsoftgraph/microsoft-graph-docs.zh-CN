---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4617e71bf0ed5d9b43e0f2d0398a0c2056e4dd1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790904"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingBusiness = await client.api('/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com')
    .version('beta')
    .get();

```