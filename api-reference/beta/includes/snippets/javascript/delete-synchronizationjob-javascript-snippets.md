---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06787edcda47fb218cd70054a3b3d710f74ba1cc5460a69b6342a94fcaa556b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/')
    .version('beta')
    .delete();

```