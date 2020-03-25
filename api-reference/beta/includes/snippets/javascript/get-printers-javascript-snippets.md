---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b719316f34a42a56e0e573e9476abd230ccef2fc
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948314"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers')
    .version('beta')
    .get();

```