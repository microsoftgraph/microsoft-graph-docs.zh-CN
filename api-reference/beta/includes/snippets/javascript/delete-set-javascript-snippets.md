---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08c3f173b422a7e3f38651b3e15d5f9c9d9b679e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/termStore/sets/{setId}')
    .version('beta')
    .delete();

```