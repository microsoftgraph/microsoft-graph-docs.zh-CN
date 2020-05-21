---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ebe2b388959ccab93b730a92f4fd2d2fd2f2888
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Video')
    .get();

```