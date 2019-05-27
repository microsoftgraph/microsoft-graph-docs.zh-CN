---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0a4c00a7e5e582f3e54d124b83943f363cc03076
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const AudioRoutingGroup = {
  id: "oneToOne",
  routingMode: "oneToOne",
  sources: [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  receivers: [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
};

let res = await client.api('/app/calls/{id}/audioRoutingGroups')
    .version('beta')
    .post({AudioRoutingGroup : AudioRoutingGroup});

```