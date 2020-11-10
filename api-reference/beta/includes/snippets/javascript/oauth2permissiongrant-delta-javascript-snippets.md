---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 593326a1cbf42c9690be1879ca3dbb41888b77ee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oauth2PermissionGrants/delta')
    .version('beta')
    .get();

```