---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cfbb178b7cdb481d0db75c38292dd76929e4b159
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .version('beta')
    .get();

```