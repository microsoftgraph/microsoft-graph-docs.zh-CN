---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75dee670b2ac8f8a1719334c085b587dc88efe54
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:wa')
    .orderby('displayName ')
    .get();

```