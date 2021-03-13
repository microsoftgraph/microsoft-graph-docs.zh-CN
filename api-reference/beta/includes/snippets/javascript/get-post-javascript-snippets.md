---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68ec8cc778d0e4a353513a69eca305ef3b9b9a0d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let post = await client.api('/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==')
    .version('beta')
    .get();

```