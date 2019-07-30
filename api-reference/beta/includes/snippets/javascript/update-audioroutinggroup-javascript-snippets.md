---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 528fbc549aa192d7a6df9a551a3ac9624f6d51d1
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933796"
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
    .update({audioRoutingGroup : audioRoutingGroup});

```