---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f23ff7001cc1f3c03ce7b91cf5003b94dea6b5954c28e010c5e5b35abe806fa6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-44b5-ae36-41b923c3bf87/resetDecisions')
    .version('beta')
    .post();

```