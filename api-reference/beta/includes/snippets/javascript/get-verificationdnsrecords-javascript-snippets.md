---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b585a3ac81e37a526011e4679617bf38b9a3ef8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800952"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let verificationDnsRecords = await client.api('/domains/contoso.com/verificationDnsRecords')
    .version('beta')
    .get();

```