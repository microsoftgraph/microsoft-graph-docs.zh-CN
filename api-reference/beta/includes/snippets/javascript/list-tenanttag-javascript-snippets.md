---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d31c18981975697f6055c9669aa8e80a65ad786
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442362"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantTags = await client.api('/tenantRelationships/managedTenants/tenantTags')
    .version('beta')
    .get();

```