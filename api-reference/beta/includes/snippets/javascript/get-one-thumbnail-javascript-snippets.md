---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 02f234567705ab4050a624d8cfd3fcbfa8e92378
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}')
    .version('beta')
    .get();

```