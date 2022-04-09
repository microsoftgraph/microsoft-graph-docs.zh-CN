---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 744c1b67da2e02a7d9d1983c82283b2a64e2f7e0
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854580"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcOrganizationSettings = await client.api('/deviceManagement/virtualEndpoint/organizationSettings')
    .version('beta')
    .get();

```