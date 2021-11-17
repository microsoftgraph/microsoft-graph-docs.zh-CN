---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e88e8f4760c9a7839e744f89bc2411b04c2600f893bcf1f1e3cb24e76bba970e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277628"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover')
    .version('beta')
    .post();

```