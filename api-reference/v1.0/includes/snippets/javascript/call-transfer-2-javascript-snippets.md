---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cfaeb0909c92bed853e3fc4fea9da8d3417a747e61b60fd6d44aeffe0d4a86e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219678"
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
        displayName: 'Heidi Steen'
      }
    },
    replacesCallId: 'e5d39592-99bd-4db8-bca8-30fb894ec51d'
  }
};

await client.api('/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer')
    .post(transfer);

```