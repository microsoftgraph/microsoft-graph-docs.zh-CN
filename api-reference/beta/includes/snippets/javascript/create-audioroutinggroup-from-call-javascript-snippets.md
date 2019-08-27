---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 76bbfb8fcddc48f72cd68a9b7b5be26aeebbb516
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636568"
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
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
};

let res = await client.api('/app/calls/{id}/audioRoutingGroups')
    .version('beta')
    .post(audioRoutingGroup);

```