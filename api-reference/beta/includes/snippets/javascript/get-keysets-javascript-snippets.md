---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34ce2d728fe1400fd6ae17c566c432239f4b245c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let keySets = await client.api('/trustFramework/keySets')
    .version('beta')
    .get();

```