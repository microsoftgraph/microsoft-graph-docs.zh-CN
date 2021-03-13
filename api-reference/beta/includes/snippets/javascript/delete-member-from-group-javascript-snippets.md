---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 069895aee7e514d249a14b94afc5f433cb6015fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{group-id}/members/{directory-object-id}/$ref')
    .version('beta')
    .delete();

```