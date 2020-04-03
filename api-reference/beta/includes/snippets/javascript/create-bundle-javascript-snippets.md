---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20a0eea5c6f4614f90256847e5a6f73e638402c6
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43127194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "Just some files",
  "@microsoft.graph.conflictBehavior" : "rename",
  bundle: { },
  children: [
    { id: "1234asdf" },
    { id: "1234qwerty" }
  ]
};

let res = await client.api('/drive/bundles')
    .version('beta')
    .post(driveItem);

```