---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ba61ab57137b0c050ee11de6ebbc3b9db8ec6115
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499537"
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