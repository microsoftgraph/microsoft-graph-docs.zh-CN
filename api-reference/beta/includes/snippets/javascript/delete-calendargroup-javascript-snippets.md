---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4901e7deaa96510295149a0ee28e41b286e1287
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .delete();

```