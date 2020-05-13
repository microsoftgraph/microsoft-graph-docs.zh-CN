---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 469b51e3d924b32743ea1a829b205abe46024bc9
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "41475712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/tokenLifetimePolicies')
    .version('beta')
    .get();

```