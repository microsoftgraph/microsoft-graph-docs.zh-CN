---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99b728787d0db88002e70a06eb3bf83772e83a39
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUserHistoryItem = await client.api('/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')
    .version('beta')
    .get();

```