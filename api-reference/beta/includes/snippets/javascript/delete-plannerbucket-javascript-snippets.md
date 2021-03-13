---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a3072920daa1d4731f21cf82ddcfaabaaaff975
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/buckets/{id}')
    .version('beta')
    .delete();

```