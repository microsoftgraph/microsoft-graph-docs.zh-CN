---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 85433c1b5affc0c799315890f274d01a884a2f78
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/content?format=%7Bformat%7D')
    .get();

```