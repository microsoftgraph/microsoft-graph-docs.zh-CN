---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 625e2eb195208fda549cae8bca6c1d13e599eea0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  key: 'Base64-encoded-pfx-content',
  password: 'password-value'
};

await client.api('/trustFramework/keySets/{id}/uploadPkcs12')
    .version('beta')
    .post(trustFrameworkKey);

```