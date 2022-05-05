---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 962d04926e248c710103cb16d89743fe1cc104a4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentRequest = {
    requestType: 'userAdd',
    assignment: {
        accessPackageId: 'd7be3253-b9c6-4fab-adef-30d30de8da2b'
    }
};

await client.api('/identityGovernance/entitlementManagement/assignmentRequests')
    .post(accessPackageAssignmentRequest);

```