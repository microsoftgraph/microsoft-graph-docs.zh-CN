---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74752607a87143b9ecb5af75ca8a9ae19b172baf
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcDevices = await client.api('/tenantRelationships/managedTenants/cloudPcDevices')
    .version('beta')
    .get();

```