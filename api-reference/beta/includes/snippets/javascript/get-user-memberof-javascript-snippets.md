---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34aa4eed21eb00f23114754ef9d1bab21efeff50
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336474"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/memberOf')
    .version('beta')
    .get();

```