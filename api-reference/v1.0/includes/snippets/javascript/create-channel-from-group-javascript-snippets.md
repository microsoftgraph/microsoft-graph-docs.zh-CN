---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9baee5663c32ba934ae21a4403fe7498245bb364
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: "Architecture Discussion",
  description: "This channel is where we debate all future architecture plans"
};

let res = await client.api('/teams/{id}/channels')
    .post({channel : channel});

```