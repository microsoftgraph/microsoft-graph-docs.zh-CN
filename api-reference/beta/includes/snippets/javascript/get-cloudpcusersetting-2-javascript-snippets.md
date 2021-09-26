---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f1e1421b4ccda774146c1e98c3dc2f7ca01c8638722627fb6904c52cfdca4c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158383"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcUserSetting = await client.api('/deviceManagement/virtualEndpoint/usersettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff')
    .version('beta')
    .expand('assignments')
    .get();

```