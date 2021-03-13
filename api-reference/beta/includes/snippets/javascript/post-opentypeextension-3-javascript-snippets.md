---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c01f791b75c1406b57d0d5656502a8fe45f2cd18
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
  '@odata.type': 'microsoft.graph.openTypeExtension',
  extensionName: 'Com.Contoso.Deal',
  companyName: 'Alpine Skis',
  dealValue: 1010100,
  expirationDate: '2015-07-03T13:04:00.000Z'
};

await client.api('/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions')
    .version('beta')
    .post(extension);

```