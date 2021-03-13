---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95539a172f3bf62c539342b6b5d993f4beaa14df
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784992"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/users/66825e03-7ef5-42da-9069-724602c31f6b/presence')
    .version('beta')
    .get();

```