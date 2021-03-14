---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d36b9b15b73ed90b150a0fcb2f6170b5fde2430
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/calendar/events')
    .get();

```