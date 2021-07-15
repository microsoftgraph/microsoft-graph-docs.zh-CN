---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29c6aca308c00e00e1a40c95f3c7bf0a902678e7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441470"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcsOverview = await client.api('/tenantRelationships/managedTenants/cloudPcsOverview')
    .version('beta')
    .get();

```