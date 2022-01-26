---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 915d6312f96fbf917ed5f1a946aee2ed9fa7fcb6
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const recordAllDecisions = {
  decision: 'Deny',
  justification: 'Alice switched teams and no longer works with this group',
  principalId: '2043848d-e422-473c-8607-88a3319ff491',
  resourceId: '733ef921-89e1-4d7e-aeff-83612223c37e'
};

await client.api('/identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')/recordAllDecisions')
    .version('beta')
    .post(recordAllDecisions);

```