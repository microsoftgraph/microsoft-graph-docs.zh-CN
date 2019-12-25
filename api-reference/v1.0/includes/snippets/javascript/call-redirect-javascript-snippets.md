---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7471d5d5618164201e7232c0e5e0e59679df0d77
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871104"
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
    .post(redirect);

```