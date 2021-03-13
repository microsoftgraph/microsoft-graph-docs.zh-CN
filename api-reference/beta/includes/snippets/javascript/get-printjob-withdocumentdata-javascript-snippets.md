---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b6f020cdf5a629123c9edf8ab4f8425ad7dceb7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printJob = await client.api('/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216')
    .version('beta')
    .expand('documents')
    .get();

```