---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc62954161e96c6e5acdba27873725b1ec908b82
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942603"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let approval = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489')
    .version('beta')
    .get();

```