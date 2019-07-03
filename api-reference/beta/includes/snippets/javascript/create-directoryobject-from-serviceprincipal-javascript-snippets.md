---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f01fa436b0cf993d6640ee393594e03cf705edac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479049"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

let res = await client.api('/servicePrincipals/{id}/owners')
    .version('beta')
    .post({directoryObject : directoryObject});

```