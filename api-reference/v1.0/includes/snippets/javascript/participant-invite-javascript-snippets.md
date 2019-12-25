---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5868a8f331cbfa5db7d415c71de11ecf6e0bcc83
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865804"
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
          displayName: "string"
        }
      }
    }
  ],
  clientContext: "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
};

let res = await client.api('/communications/calls/{id}/participants/invite')
    .post(inviteParticipantsOperation);

```