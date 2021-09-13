---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae3a071c9a18ae213c8c4f6e5bf93d9e447458f8818526cfa01648214a1590a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278621"
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
    .post(redirect);

```