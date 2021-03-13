---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffd833e1a72614f7f9cc09bf6f0af5c3ce7a9331
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{printerShareId}')
    .delete();

```