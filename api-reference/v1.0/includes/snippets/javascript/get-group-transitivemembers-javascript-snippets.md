---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9181c023e8d0f85d25048d5cea2d8d9b5369abed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMembers = await client.api('/groups/{id}/transitiveMembers')
    .get();

```