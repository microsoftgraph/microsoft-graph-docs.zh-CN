---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 349c75989bd76d25917db27dc39917279b201b5474fc9fd4e22d14609d4d9808
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902898"
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