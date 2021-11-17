---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84cca0b389f2ca66432e2a9b5bdddb31f785b25100bc1476b20d0858ff53dac0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUserHistoryItem = await client.api('/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')
    .version('beta')
    .get();

```