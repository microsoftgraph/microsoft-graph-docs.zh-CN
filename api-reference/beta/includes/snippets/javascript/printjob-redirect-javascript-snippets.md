---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 603ffa01c266177a05768db3f411f5a1751a03c1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printJob = {
  destinationPrinterId: '9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea'
};

await client.api('/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect')
    .version('beta')
    .post(printJob);

```