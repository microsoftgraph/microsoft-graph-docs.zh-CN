---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 033813bd5d120e81d5c80051ecd00345f5ba782c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776912"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printer = await client.api('/print/printers/{printerId}')
    .get();

```