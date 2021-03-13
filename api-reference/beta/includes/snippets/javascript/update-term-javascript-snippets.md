---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f25e40009c6af23f219590f1e0c52a44cdbebf6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const term = {
  labels: [
      {
          name: 'changedLabel',
          languageTag: 'en-US',
          isDefault: true
      }
  ]
};

await client.api('/termStore/sets/{setId}/terms/{termId}')
    .version('beta')
    .update(term);

```