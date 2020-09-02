---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56c709668307a931077f1cebf0c1d5b2ce337136
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const term = {
  "labels" : [
      {
          "name" : "changedLabel",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ]
};

let res = await client.api('/termStore/sets/{setId}/terms/{termId}')
    .version('beta')
    .update(term);

```