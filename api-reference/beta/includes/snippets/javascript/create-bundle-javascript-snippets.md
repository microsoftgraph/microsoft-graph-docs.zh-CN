---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1b3176fc9cf319e3f34f482d4af4bfac89e95960
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636533"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "Just some files",
  "@name.conflictBehavior" : "rename",
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