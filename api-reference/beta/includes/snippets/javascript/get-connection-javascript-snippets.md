---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58c1cbc80ee5bfa98c6f84a6332d485f829ac7bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799321"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalConnection = await client.api('/connections/contosohr')
    .version('beta')
    .get();

```