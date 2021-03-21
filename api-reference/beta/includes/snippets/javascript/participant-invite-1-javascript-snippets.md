---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5db162b22895c99a184a31d4e06b0f1e3261fe8d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inviteParticipantsOperation = {
  participants: [
    {
      '@odata.type': '#microsoft.graph.invitationParticipantInfo',
      replacesCallId: 'a7ebfb2d-871e-419c-87af-27290b22e8db',
      identity: {
        '@odata.type': '#microsoft.graph.identitySet',
        user: {
          '@odata.type': '#microsoft.graph.identity',
          id: '278405a3-f568-4b3e-b684-009193463064',
          identityProvider: 'AAD'
        }
      }
    }
  ],
  clientContext: 'f2fa86af-3c51-4bc2-8fc0-475452d9764f'
};

await client.api('/communications/calls/{id}/participants/invite')
    .version('beta')
    .post(inviteParticipantsOperation);

```