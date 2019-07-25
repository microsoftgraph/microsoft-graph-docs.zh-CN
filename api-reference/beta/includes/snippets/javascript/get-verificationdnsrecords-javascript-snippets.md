---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bc7443848049372502b239fae20d9fc0c5773eb2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/verificationDnsRecords')
    .version('beta')
    .get();

```