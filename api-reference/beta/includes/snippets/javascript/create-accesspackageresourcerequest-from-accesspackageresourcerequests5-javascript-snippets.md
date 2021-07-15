---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50445b963ba6e2f85bcc5661c1cc8e755f61391b
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRequest = {
  catalogId: 'beedadfe-01d5-4025-910b-84abb9369997',
  requestType: 'AdminRemove',
  accessPackageResource: {
    id: '354078e5-dbce-4894-8af4-0ab274d41662'
  }
};

await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```