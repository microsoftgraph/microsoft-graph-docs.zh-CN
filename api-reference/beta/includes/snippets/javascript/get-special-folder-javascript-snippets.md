---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f161b07de78b624455a17aaabcad12dae9d24a8d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{name}')
    .version('beta')
    .get();

```