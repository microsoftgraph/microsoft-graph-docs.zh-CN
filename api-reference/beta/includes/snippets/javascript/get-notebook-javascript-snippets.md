---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c2a52c88a95be8edc48538767ff0bb5448f7faf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks/{id}')
    .version('beta')
    .get();

```