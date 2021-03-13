---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f71554bf9e64219f5327319b9d60187f1163c35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/oauth2PermissionGrants/{id}')
    .version('beta')
    .delete();

```