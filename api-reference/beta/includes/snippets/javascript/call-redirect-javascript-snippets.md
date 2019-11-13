---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c7083129acafba459f60c834935bac12572dbb3
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302854"
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
        application: {
          @odata.type: "#microsoft.graph.identity",
          displayName: "test bot 2",
          id: "22bfd41f-550e-477d-8789-f6f7bd2a5e8b"
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