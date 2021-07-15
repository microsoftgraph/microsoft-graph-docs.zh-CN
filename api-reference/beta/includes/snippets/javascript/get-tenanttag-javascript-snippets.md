---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a9b531bc183ea96e1d5ff744d8e77641a8e7109
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantTag = await client.api('/tenantRelationships/managedTenants/tenantTags/{tenantTagId}')
    .version('beta')
    .get();

```