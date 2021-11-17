---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bf6e8961415ca561892c9f3ead5e6d9e3b871d21bf4f7906ce6333f7a6792e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902826"
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