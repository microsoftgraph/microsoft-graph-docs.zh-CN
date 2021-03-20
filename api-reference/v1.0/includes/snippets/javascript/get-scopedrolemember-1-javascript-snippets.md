---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e44bbe41ad15c590d978096fa6ec3af66361e81c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945577"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembership = await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .get();

```