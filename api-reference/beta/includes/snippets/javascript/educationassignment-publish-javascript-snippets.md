---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 557887a6869990c43c7376819f023f18fdc72c29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/publish')
    .version('beta')
    .post();

```