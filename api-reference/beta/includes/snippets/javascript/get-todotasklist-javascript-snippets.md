---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78543b84e4b85bafdd7784f39c9287005f1d8e26
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists')
    .version('beta')
    .get();

```