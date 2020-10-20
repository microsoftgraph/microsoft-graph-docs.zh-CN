---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea2a492f342ff0c0003eea147f7c90d90942982
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605897"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{userId}/drives')
    .version('beta')
    .get();

```