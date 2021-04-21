---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c1552b9834ac16d859dd28a33687ba2a3f61cd1
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920948"
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