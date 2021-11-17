---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 803ec3957ef1892f0ae770352dc43e9b28f5d0589295c92a1e761b4690d66efd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105174"
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