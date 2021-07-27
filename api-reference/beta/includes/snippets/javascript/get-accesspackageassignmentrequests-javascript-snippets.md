---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ff7a059586b95085687d9ed2d36a741ef02f087
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentRequests = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .filter('(requestState eq \'PendingApproval\')')
    .expand('requestor($expand=connectedOrganization)')
    .get();

```