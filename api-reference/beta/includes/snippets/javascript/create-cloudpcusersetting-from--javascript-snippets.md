---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86362d4caa00d20b5a4665da25f8cf29d763c94b46d38204ea956609408f108e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903019"
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