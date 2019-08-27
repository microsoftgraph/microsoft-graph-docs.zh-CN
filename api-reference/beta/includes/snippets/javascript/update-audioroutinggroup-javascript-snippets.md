---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dd8e987f7c477e23ab19f47d81ba28a038b3ea7d
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const audioRoutingGroup = {
  id: "oneToOne",
  routingMode: "oneToOne",
  sources: [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  receivers: [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
};

let res = await client.api('/app/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .update(audioRoutingGroup);

```