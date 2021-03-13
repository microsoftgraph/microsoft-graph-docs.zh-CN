---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11d5c65defd42bff66e46d5583ad2ea673512a2e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRequest = {
  catalogId: '26ac0c0a-08bc-4a7b-a313-839f58044ba5',
  requestType: 'AdminAdd',
  justification: '',
  accessPackageResource: {
     displayName: 'Sales',
     description: 'https://contoso.sharepoint.com/sites/Sales',
     url: 'https://contoso.sharepoint.com/sites/Sales',
     resourceType: 'SharePoint Online Site',
     originId: 'https://contoso.sharepoint.com/sites/Sales',
     originSystem: 'SharePointOnline'
  }
};

await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```