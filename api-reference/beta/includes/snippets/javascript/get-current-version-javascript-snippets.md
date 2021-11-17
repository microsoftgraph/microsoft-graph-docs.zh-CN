---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dd40dce4c614e9def70ad56e2d99fcaadf9bd68
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItemVersion = await client.api('/me/drive/items/{item-id}/versions/current')
    .version('beta')
    .get();

```