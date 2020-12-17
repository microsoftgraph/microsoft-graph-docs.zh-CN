---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 438730c3efb2fc172c2fa31d7f92a7dc0ffae261
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals')
    .version('beta')
    .get();

```