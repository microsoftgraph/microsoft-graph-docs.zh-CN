---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a97fcb9ed92ac770ccbfc1c021fe2d3c0b7cad90fda7378079de1330b561454c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158640"
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