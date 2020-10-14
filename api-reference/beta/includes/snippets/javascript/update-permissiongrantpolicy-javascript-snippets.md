---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f33fedcdcabafbd0d8ceff8ef653b8966b692659
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459610"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantPolicy = {
  displayName: "Custom permission grant policy"
};

let res = await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy')
    .version('beta')
    .update(permissionGrantPolicy);

```