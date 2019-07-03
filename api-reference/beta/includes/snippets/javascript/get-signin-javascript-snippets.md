---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fcb2eb5b2d80604694f7d8321907ade6799f69a2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns/{id}')
    .version('beta')
    .get();

```