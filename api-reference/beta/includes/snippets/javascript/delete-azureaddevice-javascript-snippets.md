---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1168b6763bc5e848817b7a91a2c488b449fe7c9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/updatableAssets/{azureADDeviceId}')
    .version('beta')
    .delete();

```