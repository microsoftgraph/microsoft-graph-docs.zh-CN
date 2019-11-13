---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 136f1f99ad6212d5200295d26079919307b122e2
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302997"
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
      replacesCallId: "a7ebfb2d-871e-419c-87af-27290b22e8db",
      identity: {
        @odata.type: "#microsoft.graph.identitySet",
        user: {
          @odata.type: "#microsoft.graph.identity",
          id: "278405a3-f568-4b3e-b684-009193463064",
          identityProvider: "AAD"
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