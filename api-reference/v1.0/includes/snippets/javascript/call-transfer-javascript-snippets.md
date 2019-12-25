---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74a5ef7faadf1ca3366ab70c3a5e07c7427e6141
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const transfer = {
  transferTarget: {
    endpointType: "default",
    identity: {
      user: {
        id: "550fae72-d251-43ec-868c-373732c2704f",
        displayName: "Heidi Steen"
      }
    },
    replacesCallId: "replacesCallId-value"
  },
  clientContext: "9e90d1c1-f61e-43e7-9f75-d420159aae08"
};

let res = await client.api('/communications/calls/{id}/transfer')
    .post(transfer);

```