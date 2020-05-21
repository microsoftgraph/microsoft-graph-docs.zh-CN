---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dc83afa8754c5ff507b47e3276b8c646e7fb54e
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/delta')
    .get();

```