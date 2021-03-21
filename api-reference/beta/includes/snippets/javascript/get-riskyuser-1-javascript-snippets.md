---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd47b126887521c79a1780b64395854a02574ccb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUser = await client.api('/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3')
    .version('beta')
    .get();

```