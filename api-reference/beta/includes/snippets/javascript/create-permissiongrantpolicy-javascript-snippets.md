---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fc5cf913e7ef19fea6d895c7626322bf9332df8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantPolicy = {
  id: 'my-custom-consent-policy',
  displayName: 'Custom application consent policy',
  description: 'A custom permission grant policy to customize conditions for granting consent.'
};

await client.api('/policies/permissionGrantPolicies')
    .version('beta')
    .post(permissionGrantPolicy);

```