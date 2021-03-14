---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ede8943fcaf1cd8b42a2f97d90a6ee953c0b35d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807655"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/unsubscribeByMail')
    .post();

```