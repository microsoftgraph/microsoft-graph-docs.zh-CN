---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3f00a6ebd9c0bc4b136cc28b66a92f4f6a7b8c1ef5fc442fd9f671d6c1ae561
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let verificationDnsRecords = await client.api('/domains/{domain-name}/verificationDnsRecords')
    .get();

```