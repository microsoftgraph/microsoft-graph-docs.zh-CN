---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3119df875d033731e5b85ce60fb2733b1df9aeb6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getEffectivePermissions = await client.api('/deviceManagement/virtualEndpoint/getEffectivePermissions')
    .version('beta')
    .get();

```