---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 867146d91976e1beba55eb7bfd00924c7b0c426e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713252"
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

let res = await client.api('/directoryRoles/{id}/members/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```