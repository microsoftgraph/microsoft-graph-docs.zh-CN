---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b276a883add7894cc6a4b58f7d655e5a1528561
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extension = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral')
    .get();

```