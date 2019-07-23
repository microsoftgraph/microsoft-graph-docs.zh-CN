---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc7f61b25a8cb62c1aee09bfb2c90ad972a85a7f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722803"
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