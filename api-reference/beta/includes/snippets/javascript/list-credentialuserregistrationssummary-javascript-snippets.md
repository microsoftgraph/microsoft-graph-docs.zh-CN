---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4033c10341e740be131f118a45596c18d775da1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let credentialUserRegistrationsSummaries = await client.api('/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries')
    .version('beta')
    .get();

```