---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93d8c31e0dc79253fc3d4a36ed4bd1df06af5ef1
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = The contents of the file goes here.;

let res = await client.api('/me/drive/items/{item-id}/content')
    .version('beta')
    .put(stream);

```