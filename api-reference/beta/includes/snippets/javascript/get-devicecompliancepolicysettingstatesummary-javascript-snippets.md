---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6da40f2cd476502386b907a35ca80496ac378dc
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439967"
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