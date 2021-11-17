---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abaf80df93626710831973e4fc53d568c6219a3931d8dbb61c71eaa5c5545b3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161567"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const domain = {
  isDefault: true,
  supportedServices: [
    'Email',
    'OfficeCommunicationsOnline'
  ]
};

await client.api('/domains/contoso.com')
    .version('beta')
    .update(domain);

```