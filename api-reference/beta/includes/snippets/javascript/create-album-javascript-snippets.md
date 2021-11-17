---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dec6418523a52940f771d98605deece0b280f96eb8588ce426321daf6e020445
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105170"
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