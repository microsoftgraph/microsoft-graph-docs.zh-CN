---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c69c6f59e22c88b6bcbe9336e8bccd57d39afe8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/root/items/016GVDAP3RCQS5VBQHORFIVU2ZMOSBL25U/extractSensitivityLabels')
    .version('beta')
    .post();

```