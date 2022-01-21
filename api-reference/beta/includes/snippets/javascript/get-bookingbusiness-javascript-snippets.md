---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec168612ab8a3c78cfe5a7857f411efe6934e99d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingBusiness = await client.api('/bookingBusinesses/Fabrikam@contoso.onmicrosoft.com')
    .version('beta')
    .get();

```