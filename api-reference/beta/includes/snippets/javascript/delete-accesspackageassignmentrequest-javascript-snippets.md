---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af5a93785b247f456380f7c54e4ab1259f5972cc
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766099"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}')
    .version('beta')
    .delete();

```