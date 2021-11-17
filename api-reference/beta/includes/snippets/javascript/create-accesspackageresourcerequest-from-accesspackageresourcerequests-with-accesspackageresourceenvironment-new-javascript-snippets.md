---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f77e69e7f4bd6b8e999560a2e2176b59fee6985b8ad1f78210b071b345b9698a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRequest = {
    catalogId: 'de9315c1-272b-4905-924b-cc112ca180c7',
    accessPackageResource: {
        displayName: 'Community Outreach',
        description: 'https://contoso.sharepoint.com/sites/CSR',
        resourceType: 'SharePoint Online Site',
        originId: 'https://contoso.sharepoint.com/sites/CSR',
        originSystem: 'SharePointOnline',
        accessPackageResourceEnvironment: {
            originId: 'https://contoso-admin.sharepoint.com/'
        }
    },
    requestType: 'AdminAdd'
};

await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```