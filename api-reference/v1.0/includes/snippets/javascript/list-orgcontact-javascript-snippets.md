---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64678ecee2da53f8ac1dc695d2ce8d462631598c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts')
    .get();

```