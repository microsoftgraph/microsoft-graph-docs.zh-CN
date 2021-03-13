---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33f23a28155f9a5b7d4090c68fe57fadc90db232
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const audioRoutingGroup = {
  id: 'oneToOne',
  routingMode: 'oneToOne',
  sources: [
    '632899f8-2ea1-4604-8413-27bd2892079f'
  ],
  receivers: [
    '550fae72-d251-43ec-868c-373732c2704f',
    '72f988bf-86f1-41af-91ab-2d7cd011db47'
  ]
};

await client.api('/communications/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .update(audioRoutingGroup);

```