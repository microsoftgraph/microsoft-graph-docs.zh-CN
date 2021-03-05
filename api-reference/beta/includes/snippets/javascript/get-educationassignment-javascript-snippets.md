---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d8b2ba5b286fef203d044e3e4511fc22fa36234
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignment = await client.api('/education/classes/11014/assignments/19002')
    .version('beta')
    .get();

```