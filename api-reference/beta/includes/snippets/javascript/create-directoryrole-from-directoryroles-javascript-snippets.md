---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4478e20df4470efce17a8b21f96198ca138dd109
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  description: 'description-value',
  displayName: 'displayName-value',
  roleTemplateId: 'roleTemplateId-value'
};

await client.api('/directoryRoles')
    .version('beta')
    .post(directoryRole);

```