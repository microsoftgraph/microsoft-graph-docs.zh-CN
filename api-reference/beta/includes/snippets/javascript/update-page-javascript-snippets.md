---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93dc8b8f032d24be306563eff2378e144a2e21023a3736f3b5889b0171ee4eec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = [
   {
    \'target\':\'#para-id\',
    \'action\':\'insert\',
    \'position\':\'before\',
    \'content\':\'<img src='image-url-or-part-name' alt='image-alt-text' />\'
  }, 
  {
    \'target\':\'#list-id\',
    \'action\':\'append\',
    \'content\':\'<li>new-page-content</li>\'
  }
];

await client.api('/me/onenote/pages/{id}/content')
    .version('beta')
    .update(stream);

```