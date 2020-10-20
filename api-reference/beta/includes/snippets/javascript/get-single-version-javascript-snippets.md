---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55ae26fb4f3dcf1d16bb55d8a8ca84fadb5f23f6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/versions/{version-id}')
    .version('beta')
    .get();

```