---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de164929c16eb3b2a398dd8bc70744225e76f796
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/dismissReminder')
    .version('beta')
    .post();

```