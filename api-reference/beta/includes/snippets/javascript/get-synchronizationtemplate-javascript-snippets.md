---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8119f2821c71fd874e68da76678d53e8e0e6a02
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let templates = await client.api('/servicePrincipals/{id}/synchronization/templates')
    .version('beta')
    .get();

```