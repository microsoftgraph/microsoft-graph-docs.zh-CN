---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f3761ef473019000a1c648a00df54ade3796e5d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335820"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName,'a'),')
    .orderby('displayName ')
    .top(1)
    .get();

```