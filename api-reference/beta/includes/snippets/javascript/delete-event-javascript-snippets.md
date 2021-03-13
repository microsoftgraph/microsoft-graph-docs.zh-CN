---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e63a22e4a765761652439bfe80e8cc18e1ed64f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}')
    .version('beta')
    .delete();

```