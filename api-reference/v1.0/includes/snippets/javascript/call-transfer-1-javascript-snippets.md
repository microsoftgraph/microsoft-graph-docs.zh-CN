---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea7ffa66462e973d06a765a52e2f5f2ffd4f2b4a
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560770"
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
    }
  }
};

await client.api('/communications/calls/{id}/transfer')
    .post(transfer);

```