---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 484054e812c1defc75126472d550ee34c20a4f36
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/calendar/events')
    .version('beta')
    .get();

```