---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbce78d1b149c2296739423e2aac2b56ec797d58
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{id}/restoreFactoryDefaults')
    .version('beta')
    .post();

```