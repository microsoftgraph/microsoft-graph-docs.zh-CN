---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c41508608b5852ca076702352e9f04f759fd34217f7d37fc3b1ab7c8da113ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute')
    .version('beta')
    .post(muteParticipantOperation);

```