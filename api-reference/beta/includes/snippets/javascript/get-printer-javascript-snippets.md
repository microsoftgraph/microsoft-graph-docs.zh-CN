---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8879730b963c59d8dff6ecedc264b039501c1c7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783459"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printer = await client.api('/print/printers/{id}')
    .version('beta')
    .get();

```