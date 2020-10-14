---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2d1ef022d65c90e11f90bc2f6ace11d584eaa46
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantConditionSet = {
  permissionType: "delegated",
  resourceApplication: "00000003-0000-0000-c000-000000000000"
};

let res = await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/excludes')
    .version('beta')
    .post(permissionGrantConditionSet);

```