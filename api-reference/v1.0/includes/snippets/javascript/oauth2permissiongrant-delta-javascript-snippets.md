---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49f5022335944f50fd1228ba97568899874ed989
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/oauth2PermissionGrants/delta')
    .get();

```