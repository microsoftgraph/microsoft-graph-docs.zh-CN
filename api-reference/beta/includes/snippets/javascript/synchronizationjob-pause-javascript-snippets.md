---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f8094203cf862c02dc2b8e450e33d970513a1d11729df644e76a27c80be08e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause')
    .version('beta')
    .post();

```