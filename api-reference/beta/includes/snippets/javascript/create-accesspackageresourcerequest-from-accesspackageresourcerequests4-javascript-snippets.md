---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12bba8f1289654d12504056d2e754707c79a4a8f830e0132d94cf3805a993894
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902764"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRequest = {

  catalogId: 'beedadfe-01d5-4025-910b-84abb9369997',
  requestType: 'AdminAdd',
  accessPackageResource: {
     originId: 'c6294667-7348-4f5a-be73-9d2c65f574f3',
     originSystem: 'AadGroup'
  }
};

await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```