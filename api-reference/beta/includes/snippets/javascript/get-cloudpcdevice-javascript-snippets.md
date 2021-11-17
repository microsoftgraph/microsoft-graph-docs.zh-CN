---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19de7ea1f58e459fcb2f1bf773bc6cc63112fcf3d4aaf83b246430b38c5a6e4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcDevice = await client.api('/tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}')
    .version('beta')
    .get();

```