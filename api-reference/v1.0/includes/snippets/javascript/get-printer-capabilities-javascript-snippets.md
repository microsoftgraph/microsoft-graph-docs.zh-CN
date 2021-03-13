---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 695b34ad1afbc9227b2ca9e4e9215b6c250dc33f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printer = await client.api('/print/printers/{printerId}')
    .select('id,displayName,capabilities')
    .get();

```