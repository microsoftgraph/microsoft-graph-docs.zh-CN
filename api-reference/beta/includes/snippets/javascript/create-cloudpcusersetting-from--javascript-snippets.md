---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a9beeb4d4f5227328b5f312f4d7c174e6fe06e9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcUserSetting = {
  '@odata.type': '#microsoft.graph.cloudPcUserSetting',
  displayName: 'Example',
  selfServiceEnabled: false,
  localAdminEnabled: true
};

await client.api('/deviceManagement/virtualEndpoint/userSettings')
    .version('beta')
    .post(cloudPcUserSetting);

```