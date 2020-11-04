---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 263fc55a048064457fc3038e2e3d73b885e45a7a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903824"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks')
    .get();

```