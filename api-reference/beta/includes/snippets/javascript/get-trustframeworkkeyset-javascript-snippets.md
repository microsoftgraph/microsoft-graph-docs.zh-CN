---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f142805b0f3fac322d66b8e1ab0f36d9032e22cc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/trustFramework/keySets/{id}')
    .version('beta')
    .get();

```