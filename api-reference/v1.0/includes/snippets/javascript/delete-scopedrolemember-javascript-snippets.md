---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2eb4e4f0ac28b5ee9577eb8e3f89be264698092
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .delete();

```