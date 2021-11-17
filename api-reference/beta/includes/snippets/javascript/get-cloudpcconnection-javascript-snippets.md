---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ef31de960d6863379f81079a4c4e5bd4283f4bafe8f519f6707da68704d7156
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcConnection = await client.api('/tenantRelationships/managedTenants/cloudPcConnections/86789ee0-e31d-4bee-98e6-6f310bd327bb')
    .version('beta')
    .get();

```