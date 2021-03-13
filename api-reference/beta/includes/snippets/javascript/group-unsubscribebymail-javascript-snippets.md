---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e5d5ded8c0c1699fe9c63ad7c09164eaddefd04
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/unsubscribeByMail')
    .version('beta')
    .post();

```