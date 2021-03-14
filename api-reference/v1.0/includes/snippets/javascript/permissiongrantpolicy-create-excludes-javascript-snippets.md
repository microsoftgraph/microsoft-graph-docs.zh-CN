---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35308053ec77a90347f8b965386c1af25e7afe7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779607"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantConditionSet = {
  permissionType: 'delegated',
  resourceApplication: '00000003-0000-0000-c000-000000000000'
};

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/excludes')
    .post(permissionGrantConditionSet);

```