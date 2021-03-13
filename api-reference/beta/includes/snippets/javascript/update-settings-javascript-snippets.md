---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4d1329422399d30ca6caf76b4c6928a6de49519
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809127"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printSettings = {
  documentConversionEnabled: true
};

await client.api('/print/settings')
    .version('beta')
    .update(printSettings);

```