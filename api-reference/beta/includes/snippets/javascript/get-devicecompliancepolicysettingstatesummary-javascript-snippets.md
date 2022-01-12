---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e32bc7c5ce6b088c511ee70f5e7e79d9146d40d95b004888298d4a6442e5f81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let response = await client.api('/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}')
    .version('beta')
    .get();

```