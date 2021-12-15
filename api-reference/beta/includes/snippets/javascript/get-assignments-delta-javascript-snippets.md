---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46d79b904bcd668018cb4355fc4ccc588b4e514b
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignment = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta')
    .version('beta')
    .get();

```