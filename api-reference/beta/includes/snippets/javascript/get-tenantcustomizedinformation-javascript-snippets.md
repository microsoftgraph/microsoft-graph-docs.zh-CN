---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5b5b4852e625d143208276a0070af907928e192
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440309"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantCustomizedInformation = await client.api('/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}')
    .version('beta')
    .get();

```