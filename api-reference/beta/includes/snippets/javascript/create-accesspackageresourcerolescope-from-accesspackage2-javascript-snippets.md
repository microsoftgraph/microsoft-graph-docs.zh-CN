---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f0ab0f9bd38fc9f6036d397799eb5e05ada90ad
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439892"
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