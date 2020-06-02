---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b719316f34a42a56e0e573e9476abd230ccef2fc
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
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