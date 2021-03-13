---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c8b325c3dca9898b5babd41914ed12e64504798
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemEmail = await client.api('/users/{userId}/profile/emails/{id}')
    .version('beta')
    .get();

```