---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcc606cf5e4f48343caa6007fab3b2463b88238e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{id}')
    .version('beta')
    .delete();

```