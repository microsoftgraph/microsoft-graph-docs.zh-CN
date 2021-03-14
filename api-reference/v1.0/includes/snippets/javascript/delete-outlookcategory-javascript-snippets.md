---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5938e911d54c01b8486a3296f8a7bd9244073d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
    .delete();

```