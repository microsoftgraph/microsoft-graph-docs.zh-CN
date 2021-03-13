---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03c66de2a96dd5a3804996cbdd439ce1ccaf47e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teachers = await client.api('/education/classes/11023/teachers')
    .version('beta')
    .get();

```