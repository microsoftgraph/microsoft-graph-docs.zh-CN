---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13b4e0faf5315c7a679e09ed4dfe2696e7228489
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let siteSettings = await client.api('/sites/03164a2b-a288-486a-993e-c41454113e2a/settings')
    .version('beta')
    .get();

```