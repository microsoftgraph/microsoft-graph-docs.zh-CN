---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afb3a634a3b18be1c19e774b25b0e8db74a68a09
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inviteParticipantsOperation = {
  participants: [
    {
      @odata.type: "#microsoft.graph.invitationParticipantInfo",
      identity: {
        @odata.type: "#microsoft.graph.identitySet",
        phone: {
          @odata.type: "#microsoft.graph.identity",
          id: "+12345678901"
        }
      }
    }
  ],
  clientContext: "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
};

let res = await client.api('/communications/calls/{id}/participants/invite')
    .version('beta')
    .post(inviteParticipantsOperation);

```