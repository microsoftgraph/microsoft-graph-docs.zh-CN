---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45295d47e9359d0dcb9684c88cc42e20049cf258
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredUsers = await client.api('/devices/{id}/registeredUsers')
    .version('beta')
    .get();

```