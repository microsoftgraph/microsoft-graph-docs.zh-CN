---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b01092dc3c90bd59f2dd4fd5d7cc0eabf3d938a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/permissionGrantPolicies/microsoft-application-admin/excludes')
    .version('beta')
    .get();

```