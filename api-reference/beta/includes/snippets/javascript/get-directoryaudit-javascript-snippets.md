---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34d9d2b0321e76dadce87cd21bff670410876ee8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryAudit = await client.api('/auditLogs/directoryAudits/{id}')
    .version('beta')
    .get();

```