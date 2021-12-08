---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c32bbbcabf099c2d74150313ff2f99a9b642b30b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantConditionSet = {
  permissionType: 'delegated',
  certifiedClientApplicationsOnly: true
};

await client.api('/policies/permissionGrantPolicies/{id}/includes')
    .version('beta')
    .post(permissionGrantConditionSet);

```