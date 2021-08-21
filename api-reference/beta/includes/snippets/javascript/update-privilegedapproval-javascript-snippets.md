---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcdf1a9e9962c8575c16acd2be4291b4a0e3d1f2e2ea4d69959353679459163f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedApproval = {
  approvalState: 'approvalState-value',
  approverReason: 'approverReason-value'
};

await client.api('/privilegedApproval/{requestId}')
    .version('beta')
    .update(privilegedApproval);

```