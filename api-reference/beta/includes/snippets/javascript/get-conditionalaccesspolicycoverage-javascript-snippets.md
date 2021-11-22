---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa92d8d4419489211acda06b4f11072afc78b66035a0f9daffa4a155013873ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conditionalAccessPolicyCoverage = await client.api('/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}')
    .version('beta')
    .get();

```