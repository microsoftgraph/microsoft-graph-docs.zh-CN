---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16772ae0e2860aec3ee774849420e0e9f9eae8de
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentRequest = await client.api('/identityGovernance/entitlementManagement/assignmentRequests/{accessPackageAssignmentRequestId}')
    .get();

```