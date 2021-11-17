---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f6b6adfcc96e93b646d21762cbafa25983a9c5750bd7c81af9a0981155602ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328822"
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
    '550fae72-d251-43ec-868c-373732c2704f'
  ]
};

await client.api('/communications/calls/{id}/audioRoutingGroups')
    .version('beta')
    .post(audioRoutingGroup);

```