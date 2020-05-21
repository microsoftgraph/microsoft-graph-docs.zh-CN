---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44a8ece3aa0c7f99c77aa54913a0593b1f3c81e6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333232"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Web')
    .get();

```