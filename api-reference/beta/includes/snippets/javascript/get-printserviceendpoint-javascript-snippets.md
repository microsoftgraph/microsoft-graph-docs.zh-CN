---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c7f74485e1a457775415dee2e0bfea460ccc90f
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/services/{id}/endpoints/{name}')
    .version('beta')
    .get();

```