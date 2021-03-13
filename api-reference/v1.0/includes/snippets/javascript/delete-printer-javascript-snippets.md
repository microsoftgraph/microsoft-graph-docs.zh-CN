---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cdf121ae49d73796ceb05f8bf6be8ad495409c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{printerId}')
    .delete();

```