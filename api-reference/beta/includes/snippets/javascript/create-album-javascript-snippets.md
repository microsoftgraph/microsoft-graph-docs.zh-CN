---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49cc5bf90997fdcbead723ace9ef73a623d9f94e
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43127222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "My Day at the Beach",
  "@microsoft.graph.conflictBehavior" : "rename",
  bundle: { album: {} },
  children: [
    { id: "1234asdf" }
  ]
};

let res = await client.api('/drive/bundles')
    .version('beta')
    .post(driveItem);

```