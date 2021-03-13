---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1679b5d81c4885348e8a3aa159f1f3d10e4ef8f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permission = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .get();

```