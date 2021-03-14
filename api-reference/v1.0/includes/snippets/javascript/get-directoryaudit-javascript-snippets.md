---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9f76e55a331d6530cec037161397ce6d25fc4bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryAudits = await client.api('/auditLogs/directoryAudits')
    .get();

```