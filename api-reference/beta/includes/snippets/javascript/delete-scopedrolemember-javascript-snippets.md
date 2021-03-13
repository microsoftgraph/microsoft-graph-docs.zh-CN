---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eaf6dcc02b68b42d95551474b96d3afec612a98
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .version('beta')
    .delete();

```