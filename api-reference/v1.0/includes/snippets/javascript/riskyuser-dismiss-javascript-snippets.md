---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 642084f452d19645a994a5f0ba76bfc9ddf62938
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  userIds: [
    '04487ee0-f4f6-4e7f-8999-facc5a30e232',
    '13387ee0-f4f6-4e7f-8999-facc5120e345'
  ]
};

await client.api('/identityProtection/riskyUsers/dismiss')
    .post(dismiss);

```