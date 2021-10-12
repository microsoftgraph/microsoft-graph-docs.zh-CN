---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d90a10770eb82f38488def9948ca7404509ec3535f1aaff3410935049f872d9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104213"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRoleScope = {
    accessPackageResourceRole: {
        originId: '4',
        originSystem: 'SharePointOnline',
        accessPackageResource: {
            id: '53c71803-a0a8-4777-aecc-075de8ee3991'
        }
    },
    accessPackageResourceScope: {
        id: '5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33',
        originId: 'https://microsoft.sharepoint.com/portals/Community',
        originSystem: 'SharePointOnline'
    }
};

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes')
    .version('beta')
    .post(accessPackageResourceRoleScope);

```