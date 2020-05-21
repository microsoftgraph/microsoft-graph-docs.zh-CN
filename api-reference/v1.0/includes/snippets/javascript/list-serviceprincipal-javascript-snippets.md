---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b829891300a99efe9b7d45ac671bacf915ace2f3
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/serviceprincipals')
    .get();

```