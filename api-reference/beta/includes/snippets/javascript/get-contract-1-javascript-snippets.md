---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd18c1c88ff5860d9e86dbbf5f990b8ccec84f46
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contract = await client.api('/contracts/{id}')
    .version('beta')
    .get();

```