---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8036bc3ff06fdd42d0502eb73bdebb9a15e20305
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/tokenLifetimePolicies/{id}/$ref')
    .version('beta')
    .delete();

```