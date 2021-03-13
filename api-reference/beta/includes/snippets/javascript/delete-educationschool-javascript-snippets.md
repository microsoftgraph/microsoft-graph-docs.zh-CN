---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eefbcdb3cd5f216750f8618271880b941900e30b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/10002')
    .version('beta')
    .delete();

```