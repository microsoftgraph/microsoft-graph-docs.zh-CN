---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5cc134fb9c118803eee7ecebeb89461851e3e7a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499730"
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