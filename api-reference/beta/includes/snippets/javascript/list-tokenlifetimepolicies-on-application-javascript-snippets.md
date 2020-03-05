---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 469b51e3d924b32743ea1a829b205abe46024bc9
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
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