---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60304b5b6910ef14f4936ed0cc40b356176df642
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441998"
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