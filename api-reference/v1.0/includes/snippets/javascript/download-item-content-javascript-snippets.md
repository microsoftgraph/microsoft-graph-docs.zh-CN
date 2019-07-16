---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c2d6a8b800a287437fc0be6b8cb29628c9620a0b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739031"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/content')
    .get();

```