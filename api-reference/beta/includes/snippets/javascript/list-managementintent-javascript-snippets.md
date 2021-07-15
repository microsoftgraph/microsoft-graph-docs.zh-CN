---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01be490629ef8d3c04ab29137ed707485e7b9dfb
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442997"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementIntents = await client.api('/tenantRelationships/managedTenants/managementIntents')
    .version('beta')
    .get();

```