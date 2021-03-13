---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d1cd3d731dbae37d5e52d2c8ec1f3bf308b0649
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const redirect = {
  targets: [
    {
      '@odata.type': '#microsoft.graph.invitationParticipantInfo',
      identity: {
        '@odata.type': '#microsoft.graph.identitySet',
        phone: {
          '@odata.type': '#microsoft.graph.identity',
          id: '+12345678901'
        }
      }
    }
  ],
  callbackUri: 'https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039'
};

await client.api('/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect')
    .version('beta')
    .post(redirect);

```