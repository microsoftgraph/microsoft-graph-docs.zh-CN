---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96ec92b17717fe2abe5614422a9072975b27d665
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516426"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let approvalStage = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/stages/d4fa4045-4716-436d-aec5-57b0a713f095')
    .get();

```