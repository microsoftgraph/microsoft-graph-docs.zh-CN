---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a50b09567d859d33f4398557428bca5083a968ce
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingCustomQuestion = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/3bc6fde0-4ad3-445d-ab17-0fc15dba0774')
    .version('beta')
    .get();

```