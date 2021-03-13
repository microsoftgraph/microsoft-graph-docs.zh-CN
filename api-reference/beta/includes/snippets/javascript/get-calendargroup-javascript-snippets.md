---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adda18b2a6c0794beae888a8ff48e73fd7d6b0c3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarGroup = await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .get();

```