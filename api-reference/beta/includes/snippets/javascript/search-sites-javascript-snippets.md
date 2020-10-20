---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba61ab57137b0c050ee11de6ebbc3b9db8ec6115
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites?search=%7Bquery%7D')
    .version('beta')
    .get();

```