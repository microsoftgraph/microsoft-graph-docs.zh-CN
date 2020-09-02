---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ff465e9877613b164731227362105d5b3a5704e
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const term = {
  labels: [
    {
      "languageTag" : "en-US",
      "name" : "Car",
      "isDefault" : true
    }
  ]
};

let res = await client.api('/termStore/sets/{setId}/terms')
    .version('beta')
    .post(term);

```