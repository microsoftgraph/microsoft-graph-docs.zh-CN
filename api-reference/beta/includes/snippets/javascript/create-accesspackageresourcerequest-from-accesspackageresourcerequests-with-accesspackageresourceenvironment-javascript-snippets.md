---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acec89281484aa2ecbb541d2ed4d80321df8d7444183d3f83af55013e0ee3afb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902765"
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
        'accessPackageResourceEnvironment@odata.bind': 'accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57'
    },
    requestType: 'AdminAdd'
};

await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```