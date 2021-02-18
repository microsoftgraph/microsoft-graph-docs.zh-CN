---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9277f2263f0254a140191c2b8b3ac6487de89371
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const redirect = {
  targets: [
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
  callbackUri: "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
};

let res = await client.api('/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect')
    .post(redirect);

```