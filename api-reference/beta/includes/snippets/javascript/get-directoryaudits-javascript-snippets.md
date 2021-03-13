---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f42bbe1c5af2b0ac2588310d313f490e14238745
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782003"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryAudits = await client.api('/auditLogs/directoryAudits')
    .version('beta')
    .get();

```