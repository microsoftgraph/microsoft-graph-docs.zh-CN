---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f90440934085159e106691280c894de4f33a58e7
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/serviceprincipals/{id}/owners/{id}/$ref')
    .delete();

```