---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b57d835f5fec68aea3ae5df9ec45485d78bc0c60
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440179"
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