---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79750707dc1b186e5d6e34dc06c578bc45bb9bc4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/sendReminder')
    .version('beta')
    .post();

```