---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26f870cbe04152b1229ce3aa4a1883e5a1cc95eb66f2431143dbf01b8fcb05d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104330"
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
    }
  ],
  clientContext: 'f2fa86af-3c51-4bc2-8fc0-475452d9764f'
};

await client.api('/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants/invite')
    .post(inviteParticipantsOperation);

```