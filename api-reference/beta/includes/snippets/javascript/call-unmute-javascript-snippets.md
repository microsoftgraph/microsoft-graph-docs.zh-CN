---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 926ea5aefce85ff7e5cf54aeeca6d43e2cdd0599
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779611"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unmuteParticipantOperation = {
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute')
    .version('beta')
    .post(unmuteParticipantOperation);

```