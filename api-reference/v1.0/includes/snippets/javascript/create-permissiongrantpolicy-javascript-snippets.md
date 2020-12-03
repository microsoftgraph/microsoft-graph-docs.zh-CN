---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4926487de999cbd5b261437ac00db3a64e4faab3
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524114"
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
    .post(permissionGrantPolicy);

```