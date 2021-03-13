---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44a5fd82924ef9f171c7eadc492b329cdd7b8944
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'Just some files',
  '@microsoft.graph.conflictBehavior': 'rename',
  bundle: { },
  children: [
    { id: '1234asdf' },
    { id: '1234qwerty' }
  ]
};

await client.api('/drive/bundles')
    .version('beta')
    .post(driveItem);

```