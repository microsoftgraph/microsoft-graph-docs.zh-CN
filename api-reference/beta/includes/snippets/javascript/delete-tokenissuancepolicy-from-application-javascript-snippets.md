---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f7ad51c87d81300a4d94a440a5d67d2380e62d6
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/tokenIssuancePolicies/{id}/$ref')
    .version('beta')
    .delete();

```