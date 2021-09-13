---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c70b3b90d0e5b4403087c919d5d9115e42f16317ff5296ec38b7bf5b38361138
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104331"
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
          id: '7e1b4346-85a6-4bdd-abe3-d11c5d420efe',
          displayName: 'string'
        }
      }
    },
    {
      '@odata.type': '#microsoft.graph.invitationParticipantInfo',
      replacesCallId: 'a7ebfb2d-871e-419c-87af-27290b22e8db',
      identity: {
        '@odata.type': '#microsoft.graph.identitySet',
        user: {
          '@odata.type': '#microsoft.graph.identity',
          id: '1e126418-44a0-4a94-a6f8-0efe1ad71acb',
          displayName: 'string'
        }
      }
    }
  ],
  clientContext: 'f2fa86af-3c51-4bc2-8fc0-475452d9764f'
};

await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/invite')
    .post(inviteParticipantsOperation);

```