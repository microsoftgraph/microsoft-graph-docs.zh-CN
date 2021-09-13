---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16e2144365cf6c52b2946f8aa9a8698b2935a7be5c8a9c8a8c679047f3ae576d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const transfer = {
  transferTarget: {
    '@odata.type': '#microsoft.graph.invitationParticipantInfo',
    endpointType: 'default',
    identity: {
      '@odata.type': '#microsoft.graph.identitySet',
        phone: {
          '@odata.type': '#microsoft.graph.identity',
          id: '+12345678901'
        }
    },
    languageId: 'en-us',
    region: 'amer',
    replacesCallId: 'e5d39592-99bd-4db8-bca8-30fb894ec51d'
  },
  clientContext: '9e90d1c1-f61e-43e7-9f75-d420159aae08'
};

await client.api('/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer')
    .post(transfer);

```