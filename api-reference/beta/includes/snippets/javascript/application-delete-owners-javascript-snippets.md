---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e27be6dcb43c711ef55d4189c916bf9a171ebabd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789420"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/owners/{id}/$ref')
    .version('beta')
    .delete();

```