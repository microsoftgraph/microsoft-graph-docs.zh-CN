---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f721c52310355f731dfa4b45eeab1fa39cc5d5ca8b31e1c904b646a2a8e09296
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219677"
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
        displayName: 'Heidi Steen'
      }
    },
    replacesCallId: 'replacesCallId-value'
  }
};

await client.api('/communications/calls/{id}/transfer')
    .post(transfer);

```