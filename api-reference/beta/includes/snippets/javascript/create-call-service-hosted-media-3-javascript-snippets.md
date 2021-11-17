---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbe45432896155d02b4b88a234ca23153dfc350a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  '@odata.type': '#microsoft.graph.call',
  callbackUri: 'https://bot.contoso.com/callback',
  source: {
    '@odata.type': '#microsoft.graph.participantInfo',
    identity: {
      '@odata.type': '#microsoft.graph.identitySet',
      applicationInstance: {
        '@odata.type': '#microsoft.graph.identity',
        displayName: 'Calling Bot',
        id: '3d913abb-aec0-4964-8fa6-3c6850c4f278'
      }
    },
    countryCode: null,
    endpointType: null,
    region: null,
    languageId: null
  },
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
  requestedModalities: [
    'audio'
  ],
  mediaConfig: {
    '@odata.type': '#microsoft.graph.appHostedMediaConfig',
    blob: '<Media Session Configuration>'
  },
  tenantId: 'aa67bd4c-8475-432d-bd41-39f255720e0a'
};

await client.api('/communications/calls')
    .version('beta')
    .post(call);

```