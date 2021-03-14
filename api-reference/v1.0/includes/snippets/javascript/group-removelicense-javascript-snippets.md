---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03ad6a203acdcddcc3cddaf48ee1c5577626e2d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  addLicenses: [],
  removeLicenses: ['skuId-value-1', 'skuId-value-2']
};

await client.api('/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense')
    .post(group);

```