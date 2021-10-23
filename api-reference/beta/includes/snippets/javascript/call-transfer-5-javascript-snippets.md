---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e88fccebb9fdb6ced9a3746388d505bcc52dcfe
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561582"
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
  },
  transferee: {
    identity: {
      user: {
        id: '751f6800-3180-414d-bd94-333364659951',
        tenantId: '72f988bf-86f1-41af-91ab-2d7cd011db47'
      }
    },
    participantId: '909c6581-5130-43e9-88f3-fcb3582cde37'
  },
  languageId: 'languageId-value',
  region: 'region-value'
};

await client.api('/communications/calls/{id}/transfer')
    .version('beta')
    .post(transfer);

```