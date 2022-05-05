---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: affba4df1c246861c356c43fb07a38a074d9106f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const confirmSafe = {
  requestIds: [
    '5a0c76d2-cb57-4ece-9bc1-c323178f116a',
    '96609214-09ef-4f80-9d4a-ace5fceecaec',
    '05020696-4eb8-45a3-918f-8f8bb7ad6015'
  ]
};

await client.api('/auditLogs/signIns/confirmSafe')
    .version('beta')
    .post(confirmSafe);

```