---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c06adb4c55d702b6158c3d82e7c231863d51d78
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768875"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationTemplate = await client.api('/applicationTemplates/{id}')
    .get();

```