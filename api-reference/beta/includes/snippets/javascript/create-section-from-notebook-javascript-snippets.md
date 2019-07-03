---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d9e70ededb5507a7c61f24898dc33aad3925f0b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: "Section name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sections')
    .version('beta')
    .post({onenoteSection : onenoteSection});

```