---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 424b1e767266c5465b5c9b06bab827865dff6d1e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentSharingSessions = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/contentSharingSessions')
    .version('beta')
    .get();

```