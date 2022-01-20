---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73acbf198aa2cae46e6faf2ebf437f592006aad4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingStaffMember = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51')
    .version('beta')
    .get();

```