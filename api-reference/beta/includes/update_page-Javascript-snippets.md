---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 819318934baf928978419467e3f474584ffce711
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Stream = [
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
];

let res = await client.api('/me/onenote/pages/{id}/content')
    .version('beta')
    .update({Stream : Stream});

```