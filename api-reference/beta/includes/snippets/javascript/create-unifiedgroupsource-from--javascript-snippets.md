---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 600c97c445773ec087b4eb08b1ede7097f11e619
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedGroupSource = {
    'group@odata.bind': 'https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610',
    includedSources: 'mailbox'
};

await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/unifiedGroupSources')
    .version('beta')
    .post(unifiedGroupSource);

```