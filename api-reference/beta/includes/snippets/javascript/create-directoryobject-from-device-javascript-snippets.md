---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5cc134fb9c118803eee7ecebeb89461851e3e7a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706945"
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

let res = await client.api('/devices/{id}/registeredUsers/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```