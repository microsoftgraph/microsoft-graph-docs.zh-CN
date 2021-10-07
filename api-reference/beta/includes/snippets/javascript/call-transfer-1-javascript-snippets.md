---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d271b7a4ef4f34d65df8cb44a9fa4a0e80b762ad06ee25681f6c413ac780ca3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const transfer = {
  transferTarget: {
    endpointType: 'default',
    identity: {
      user: {
        id: '550fae72-d251-43ec-868c-373732c2704f',
        tenantId: '72f988bf-86f1-41af-91ab-2d7cd011db47',
        displayName: 'Heidi Steen'
      }
    },
    languageId: 'languageId-value',
    region: 'region-value'
  }
};

await client.api('/communications/calls/{id}/transfer')
    .version('beta')
    .post(transfer);

```