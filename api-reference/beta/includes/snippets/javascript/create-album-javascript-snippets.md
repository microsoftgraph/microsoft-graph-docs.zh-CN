---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f37b252e92002bc3f8872ee9dd90eada416cbbaa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'My Day at the Beach',
  '@microsoft.graph.conflictBehavior': 'rename',
  bundle: { album: {} },
  children: [
    { id: '1234asdf' }
  ]
};

await client.api('/drive/bundles')
    .version('beta')
    .post(driveItem);

```