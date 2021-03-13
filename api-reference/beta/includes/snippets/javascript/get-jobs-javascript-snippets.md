---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07857ecac9c6c64a0728859fdf3e88ebe31faacc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/servicePrincipals/{id}/synchronization/jobs/')
    .version('beta')
    .get();

```