---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e1556378ed2bd54d4e513484a2469232949fcc8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/resetUnseenCount')
    .version('beta')
    .post();

```