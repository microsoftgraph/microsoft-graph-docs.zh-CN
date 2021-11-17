---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13c7cae92e50ca3ffd071b26aafd8c629d7f1c1252a07ed9dd57d2dde8a3a0ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332726"
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