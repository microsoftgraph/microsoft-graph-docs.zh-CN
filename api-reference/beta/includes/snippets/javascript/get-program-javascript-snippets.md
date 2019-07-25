---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7b99c3dff2098cae61f03ffefe988bfa660cc84b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720074"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programs')
    .version('beta')
    .get();

```