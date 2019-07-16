---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2899d5e46380611c0f266d35e0cc4d198289795b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/{object-id}/restore')
    .post();

```