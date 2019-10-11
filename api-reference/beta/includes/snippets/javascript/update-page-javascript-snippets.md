---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6ec02de37009e3440b97543112fdf9a9e4eb35e
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = [
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
    .update(stream);

```