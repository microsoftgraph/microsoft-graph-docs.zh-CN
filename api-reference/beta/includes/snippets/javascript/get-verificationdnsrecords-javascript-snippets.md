---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40e4d169cab46d6f83d31a245ba432b2df95db33b7039a0a5974b981792e748d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104819"
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