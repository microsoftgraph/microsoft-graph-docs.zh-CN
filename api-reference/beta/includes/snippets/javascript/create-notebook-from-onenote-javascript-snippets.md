---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dd13612a9e39d620b897c5d63d2ca748427d60b6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
  displayName: "Notebook name"
};

let res = await client.api('/me/onenote/notebooks')
    .version('beta')
    .post({notebook : notebook});

```