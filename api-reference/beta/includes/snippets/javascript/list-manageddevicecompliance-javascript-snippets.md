---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb1ae72b2ccdc38a2f4c2bd4ee3dd970d86d23fae417f26a7ff7d8ff405f5b13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managedDeviceCompliances = await client.api('/tenantRelationships/managedTenants/managedDeviceCompliances')
    .version('beta')
    .get();

```