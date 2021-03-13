---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93196396d61cb146c4b518414b8c59b79fa0f7ab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802149"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
  '@odata.type': 'microsoft.graph.openTypeExtension',
  extensionName: 'Com.Contoso.Referral',
  companyName: 'Wingtip Toys',
  dealValue: 500050,
  expirationDate: '2015-12-03T10:00:00.000Z'
};

await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions')
    .version('beta')
    .post(extension);

```