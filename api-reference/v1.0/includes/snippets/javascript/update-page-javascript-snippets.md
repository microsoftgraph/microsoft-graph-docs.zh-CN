---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b054481a8e6613cae8d3ea761484863e32fedd13
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810209"
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
    .update(stream);

```