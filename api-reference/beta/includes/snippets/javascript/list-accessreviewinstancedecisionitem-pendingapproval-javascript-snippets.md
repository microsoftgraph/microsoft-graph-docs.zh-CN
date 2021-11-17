---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a87bef327902f80b0184d291455bf81ee4df4c65db19e2130fdb0c90d0da800d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let decisions = await client.api('/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```