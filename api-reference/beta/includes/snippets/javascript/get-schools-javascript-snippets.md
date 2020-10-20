---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97a50d98be2d4640d690af7ea35e5d6ed0055eb5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/schools')
    .version('beta')
    .get();

```