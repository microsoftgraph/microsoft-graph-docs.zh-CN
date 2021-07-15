---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a6a0e336046ae9f14ac0b95e62e8e48e929df8f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let credentialUserRegistrationsSummary = await client.api('/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}')
    .version('beta')
    .get();

```