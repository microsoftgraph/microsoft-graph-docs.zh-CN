---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 837895e988dc43d86f6de92ede6a9ef6eb979724
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementTemplate = await client.api('/tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}')
    .version('beta')
    .get();

```