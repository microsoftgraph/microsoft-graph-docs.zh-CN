---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 295a20f92dfa4730c95eacfadad17cdead11baa25a34191fd710be1f80dc3d7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff')
    .version('beta')
    .delete();

```