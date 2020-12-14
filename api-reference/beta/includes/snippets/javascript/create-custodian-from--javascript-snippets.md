---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49236c26c73d9a66f226e3217220fcd0c922a9a0
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const custodian = {
    email:"AdeleV@contoso.com",
    applyHoldToSources:"true"
};

let res = await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians')
    .version('beta')
    .post(custodian);

```