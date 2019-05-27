---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc7f61b25a8cb62c1aee09bfb2c90ad972a85a7f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "Self help community for library",
  displayName: "Library Assist",
  groupTypes: [
    "Unified"
  ],
  mailEnabled: true,
  mailNickname: "library",
  securityEnabled: false
};

let res = await client.api('/groups')
    .post({group : group});

```