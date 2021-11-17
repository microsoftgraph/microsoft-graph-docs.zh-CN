---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3b24f707d8e1e42dda5c524501239eb9d056f8513d56a60383a382da0e06604
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let aggregatedPolicyCompliances = await client.api('/tenantRelationships/managedTenants/aggregatedPolicyCompliances')
    .version('beta')
    .get();

```