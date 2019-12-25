---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c1d04cf79a21b9b3724569c035def2e2a284c49
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865819"
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
          id: "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          displayName: "string"
        }
      }
    }
  ],
  clientContext: "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
};

let res = await client.api('/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants/invite')
    .post(inviteParticipantsOperation);

```