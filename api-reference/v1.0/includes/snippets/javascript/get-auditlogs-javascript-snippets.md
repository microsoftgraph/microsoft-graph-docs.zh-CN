---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a45f7b401219ed327d318dc72e8a6fceb5b875ef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let auditLogRoot = await client.api('/auditLogs')
    .get();

```