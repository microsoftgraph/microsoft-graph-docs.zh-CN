---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad6c7918c60862f56c34c53924cb7342d8d61be7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443070"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementTemplates = await client.api('/tenantRelationships/managedTenants/managementTemplates')
    .version('beta')
    .get();

```