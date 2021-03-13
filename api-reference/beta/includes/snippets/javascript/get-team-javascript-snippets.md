---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bbfcf7843af21a20ade4e409fd023a64d241f3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let team = await client.api('/teams/{id}')
    .version('beta')
    .get();

```