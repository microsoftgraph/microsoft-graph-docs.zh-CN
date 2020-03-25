---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7f3d018d202d86f28d84d03b6c303ba227f2154
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  name: "name-value",
  printer@odata.bind: "https://graph.microsoft.com/beta/print/printers/{id}"
};

let res = await client.api('/print/printerShares')
    .version('beta')
    .post(printerShare);

```