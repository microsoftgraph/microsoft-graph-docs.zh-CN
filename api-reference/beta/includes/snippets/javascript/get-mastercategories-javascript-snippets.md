---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49504510d4fdf6fc4a5f9dd226a361d666272bd8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let masterCategories = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .get();

```