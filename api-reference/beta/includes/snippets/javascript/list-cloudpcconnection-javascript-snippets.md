---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ed1788be025d548b8de11e357712279eee106a5
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441572"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcConnections = await client.api('/tenantRelationships/managedTenants/cloudPcConnections')
    .version('beta')
    .get();

```