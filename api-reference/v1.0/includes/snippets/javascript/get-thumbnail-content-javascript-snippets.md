---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 21363560b6efd0e3e9909158cc012ee433ac9410
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content')
    .get();

```