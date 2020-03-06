---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9f9ad1143c1bd9f3eb4bfa1e9eee2de3b3846f7
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const domain = {
  isDefault: true,
  supportedServices: [
    "Email",
    "OfficeCommunicationsOnline"
  ]
};

let res = await client.api('/domains/contoso.com')
    .update(domain);

```