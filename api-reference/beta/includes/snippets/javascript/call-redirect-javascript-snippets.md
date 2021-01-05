---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30aff109adec0f7436c93b7b27979e2b2b4db19e
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756002"
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
    .version('beta')
    .post(redirect);

```