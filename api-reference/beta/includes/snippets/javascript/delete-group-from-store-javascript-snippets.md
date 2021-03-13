---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a14c009d58a80e1660c296a2bae719a4ed12a9d4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/termStore/groups/{groupId}')
    .version('beta')
    .delete();

```