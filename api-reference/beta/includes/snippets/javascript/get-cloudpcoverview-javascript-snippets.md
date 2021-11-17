---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02c9b20f35e1e82547a5b9478bc189a9a6b1d479132caac3e305d8c2e1ee3ff6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcOverview = await client.api('/tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}')
    .version('beta')
    .get();

```