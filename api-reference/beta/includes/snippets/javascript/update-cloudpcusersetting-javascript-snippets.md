---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddce108d42f12fd78f1c2d4b8556de52d437f88547a5b3ad07bca48b76c6bc75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcUserSetting = {
  '@odata.type': '#microsoft.graph.cloudPcUserSetting',
  displayName: 'Example',
  selfServiceEnabled: true,
  localAdminEnabled: false
};

await client.api('/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff')
    .version('beta')
    .update(cloudPcUserSetting);

```