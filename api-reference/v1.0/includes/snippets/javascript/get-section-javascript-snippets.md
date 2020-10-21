---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72e71a3dec0f4f02a7fbee1e869eb7407c24e8f3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sections/{id}')
    .get();

```