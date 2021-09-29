---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58f53af7b6abd9d7f883dacc6e6e4db15111afe5
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .header('ConsistencyLevel','eventual')
    .filter('mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq \'Unified\')) and membershipRuleProcessingState eq \'On\'')
    .select('id,membershipRule,membershipRuleProcessingState')
    .get();

```