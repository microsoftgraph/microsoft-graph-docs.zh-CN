---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96a87d0c109534a5de8580aaaf92f6e2561cc7da
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let participants = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants')
    .version('beta')
    .get();

```