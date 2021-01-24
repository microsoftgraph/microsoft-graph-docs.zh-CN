---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d50a8d5785d9b6c864494d7e05007c5e710a7cc5
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945706"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .get();

```