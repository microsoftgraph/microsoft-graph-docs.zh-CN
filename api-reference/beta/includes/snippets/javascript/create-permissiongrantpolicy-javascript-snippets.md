---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66bf280f3f81708c12a65123436a7e6458584183
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantPolicy = {
  id: "my-custom-consent-policy",
  displayName: "Custom application consent policy",
  description: "A custom permission grant policy to customize conditions for granting consent."
};

let res = await client.api('/policies/permissionGrantPolicies')
    .version('beta')
    .post(permissionGrantPolicy);

```