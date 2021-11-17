---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49f5cb1e5fb6b9ed7935fe7f4971a87ae1daf66c855532acc20125e673674541
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementActions = await client.api('/tenantRelationships/managedTenants/managementActions')
    .version('beta')
    .get();

```