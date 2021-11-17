---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2cb7bda14b16c7d921c76cf3d27dface15ab9745ed056708dfd3e8b79e92443
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902766"
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