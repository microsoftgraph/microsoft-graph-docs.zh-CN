---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6bea74cde4e0f7587edb49c65b35821477d9a8021a9d07a85491d985bdec820
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219602"
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