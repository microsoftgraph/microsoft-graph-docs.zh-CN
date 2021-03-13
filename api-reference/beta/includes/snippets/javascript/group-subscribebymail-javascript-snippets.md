---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce1b2e39c0df37ae96d690d51e074bd4dfef791b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/subscribeByMail')
    .version('beta')
    .post();

```