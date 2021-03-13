---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aa41ba1561fb823d2b71c02733b7b2e2bf5be79
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806191"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let provisioning = await client.api('/auditLogs/provisioning')
    .version('beta')
    .get();

```