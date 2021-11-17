---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 640df51d6aa2f56d5db1377e02f92e22359a4e5720dd4d5a29083b99cb851ce1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158595"
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