---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3a92e8cb4f8cf4515730c273a6cec363e698c64
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedUsers = await client.api('/print/shares/{id}/allowedUsers')
    .version('beta')
    .get();

```