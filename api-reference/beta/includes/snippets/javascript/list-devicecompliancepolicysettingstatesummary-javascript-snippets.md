---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3820a09b23711ddedb9b3a18d0164e629373a1ef5e754221110279b5f6d3f8ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deviceCompliancePolicySettingStateSummary = await client.api('/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary')
    .version('beta')
    .get();

```