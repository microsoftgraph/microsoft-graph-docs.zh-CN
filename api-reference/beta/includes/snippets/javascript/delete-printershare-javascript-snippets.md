---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4532e548f63b491c9123280fc993dddb0f1ab0f5
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947697"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printerShares/{id}')
    .version('beta')
    .delete();

```