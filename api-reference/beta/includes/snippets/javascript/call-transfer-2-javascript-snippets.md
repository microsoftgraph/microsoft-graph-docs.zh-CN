---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ecc93ba9ff036e57be41a54138ebabdb681db57
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921012"
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
      user: {
        '@odata.type': '#microsoft.graph.identity',
        id: '550fae72-d251-43ec-868c-373732c2704f',
        tenantId: '72f988bf-86f1-41af-91ab-2d7cd011db47',
        displayName: 'Heidi Steen'
      }
    },
    languageId: 'en-us',
    region: 'amer',
    replacesCallId: 'e5d39592-99bd-4db8-bca8-30fb894ec51d'
  }
};

await client.api('/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer')
    .version('beta')
    .post(transfer);

```