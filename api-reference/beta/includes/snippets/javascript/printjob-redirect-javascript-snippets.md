---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cca16f4c1308c371c1fcb5a052f22fdd805ede22
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printJob = {
  destinationPrinterId: "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea"
};

let res = await client.api('/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect')
    .version('beta')
    .post(printJob);

```