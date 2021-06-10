---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9312091486525967b084a51590c8d1fdaa56fa05
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473613"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentRequest = {
    requestType: 'UserAdd',
    accessPackageAssignment: {
        accessPackageId: 'a914b616-e04e-476b-aa37-91038f0b165b'
    },
    justification: 'Need access to New Hire access package'
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .post(accessPackageAssignmentRequest);

```