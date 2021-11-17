---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aeac8396319fa279ae316c4364c9d0f0dcd4967e28f31cca12c58a00db3a2297
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164110"
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