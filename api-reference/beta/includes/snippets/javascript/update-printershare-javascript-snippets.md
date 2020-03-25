---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c31f55bbe053dd56f65dc5d7daaa33570d2b2306
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  name: "ShareName",
  printer@odata.bind: "https://graph.microsoft.com/beta/print/printers/{id}"
};

let res = await client.api('/print/printerShares/{id}')
    .version('beta')
    .update(printerShare);

```