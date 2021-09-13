---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f273384fdef1021d25c7cc8d607b21453b85a77275160da69f6b8a0b1d2a5b92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .delete();

```