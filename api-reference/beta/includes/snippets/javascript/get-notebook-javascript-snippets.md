---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c2a52c88a95be8edc48538767ff0bb5448f7faf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479146"
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