---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ac73bfdf915523746b5a9e8d98fbe5f4ded78307950845637c42cee366f8bc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220974"
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