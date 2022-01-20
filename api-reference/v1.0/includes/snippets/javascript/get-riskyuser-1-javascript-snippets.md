---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cb3a41b3b9027a46ff23e9403f1133a1b4d051b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132127"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUser = await client.api('/identityProtection/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3')
    .get();

```