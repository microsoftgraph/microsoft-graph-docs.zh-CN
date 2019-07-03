---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6ed7779e22fbc5452d7d6b2adc0963855ecf232e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478267"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/analytics')
    .version('beta')
    .get();

```