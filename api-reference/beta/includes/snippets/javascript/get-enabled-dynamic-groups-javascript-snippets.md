---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f439b23764e19955eb36cf7970b660663aa8d56
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59998187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .version('beta')
    .filter('mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq \'Unified\')) and membershipRuleProcessingState eq \'On\'')
    .select('id,membershipRule,membershipRuleProcessingState')
    .get();

```