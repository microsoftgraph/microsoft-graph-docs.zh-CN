---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 171dc89cea191fce78b2dd7fd313570c75bcae89
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516452"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let approval = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489')
    .get();

```