---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19bad9b1951e78241bc99ae51ecc94e3cdecaa4289cbf673f269c41de0b24e80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentRequest = {
    requestType: 'AdminRemove',
    accessPackageAssignment: {
     id: 'a6bb6942-3ae1-4259-9908-0133aaee9377'
    }
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .post(accessPackageAssignmentRequest);

```