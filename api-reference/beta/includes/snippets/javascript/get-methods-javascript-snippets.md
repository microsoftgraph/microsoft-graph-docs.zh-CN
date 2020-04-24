---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78e47fe1eb6fb4bff38559784f8e35b599a510ae
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/methods')
    .version('beta')
    .get();

```