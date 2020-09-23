---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23b556dffde29f24c2469327d102d5ca291f0401
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/continuousAccessEvaluationPolicy')
    .version('beta')
    .get();

```