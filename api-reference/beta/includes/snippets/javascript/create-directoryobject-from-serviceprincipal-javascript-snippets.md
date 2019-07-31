---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f01fa436b0cf993d6640ee393594e03cf705edac
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717650"
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