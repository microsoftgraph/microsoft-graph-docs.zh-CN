---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ab483d9d5ca57cfe37e727033996246950534d626114a1807b9e6148511cd62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378627"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}')
    .version('beta')
    .delete();

```