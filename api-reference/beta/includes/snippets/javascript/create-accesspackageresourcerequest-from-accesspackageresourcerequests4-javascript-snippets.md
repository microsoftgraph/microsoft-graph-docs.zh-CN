---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6eb57c1a32302b0c2183b5dc7fd38e88e8d9e3ab
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439142"
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