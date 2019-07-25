---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6a288ed7f335a04247fbca11a2da80db607076b6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/delta')
    .version('beta')
    .get();

```