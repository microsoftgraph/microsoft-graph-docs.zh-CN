---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44a5fd82924ef9f171c7eadc492b329cdd7b8944
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757670"
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