---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85841ef9d9cad8ea0d3c6a3f7db90ca75fe3e64794f0ad3e769aa79b349f172a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103816"
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