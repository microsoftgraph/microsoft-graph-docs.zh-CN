---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8c471e9767ecfa7731744cf53164f365d1fee45cf016b60d43c58d3d976240b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279141"
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