---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9f35ac4f2c694a572c0d4623dcbeb8a8fc34290
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/compliance/ediscovery/cases')
    .version('beta')
    .get();

```