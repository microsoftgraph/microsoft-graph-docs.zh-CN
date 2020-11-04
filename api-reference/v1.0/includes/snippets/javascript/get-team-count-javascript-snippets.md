---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44bc9476ca230fac913255f19bedaac76ded6a91
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Team')
    .get();

```