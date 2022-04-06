---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc236bd2dd3a7b6c8a5ff5bcc1a00d67ff79e49f
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515824"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/filterByCurrentUser(on='approver')')
    .get();

```