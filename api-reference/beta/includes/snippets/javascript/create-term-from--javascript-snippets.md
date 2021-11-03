---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 803006c43a1e2030f0a587872f651aba05444cac
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60718095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const term = {
  labels: [
    {
      languageTag: 'en-US',
      name: 'Car',
      isDefault: true
    }
  ]
};

await client.api('/termStore/sets/{setId}/children')
    .version('beta')
    .post(term);

```