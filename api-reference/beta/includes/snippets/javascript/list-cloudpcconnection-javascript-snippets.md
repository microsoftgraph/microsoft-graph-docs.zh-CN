---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bd48245dca7130555b33f424185ff3b74f1c30ff0a405dbeb1d11d156375491
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcConnections = await client.api('/tenantRelationships/managedTenants/cloudPcConnections')
    .version('beta')
    .get();

```