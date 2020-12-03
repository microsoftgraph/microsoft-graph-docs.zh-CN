---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f63baf8b8b35d48098e896acd9bf86ba957fc9e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524207"
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
    .post(permissionGrantConditionSet);

```