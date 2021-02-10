---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22c4638a2089da5a1f0b20bfe0d12a92b921558e
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRequest = {
    catalogId: "de9315c1-272b-4905-924b-cc112ca180c7",
    accessPackageResource: {
        displayName: "Community Outreach",
        description: "https://contoso.sharepoint.com/sites/CSR",
        resourceType: "SharePoint Online Site",
        originId: "https://contoso.sharepoint.com/sites/CSR",
        originSystem: "SharePointOnline",
        accessPackageResourceEnvironment: {
            originId: "https://contoso-admin.sharepoint.com/"
        }
    },
    requestType: "AdminAdd"
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```