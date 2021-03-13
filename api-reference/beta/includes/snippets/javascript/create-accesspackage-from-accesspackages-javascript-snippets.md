---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e233a79bacb8204e6160f2084dec312381b2d8ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackage = {
  catalogId: 'aa2f6514-3232-46e7-a08a-2411ad8d7128',
  displayName: 'sales reps',
  description: 'outside sales representatives'
};

await client.api('/identityGovernance/entitlementManagement/accessPackages')
    .version('beta')
    .post(accessPackage);

```