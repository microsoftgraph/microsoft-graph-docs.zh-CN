---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f5be1b5195cfdd9fd07ec14232d9d664565a4d46
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/directoryAudits/{id}')
    .version('beta')
    .get();

```