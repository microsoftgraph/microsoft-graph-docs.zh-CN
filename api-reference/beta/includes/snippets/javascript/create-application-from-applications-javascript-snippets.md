---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fe137b6cfb2a5cb33800ac9bdf5e1a56f9a5aa4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: 'Display name'
};

await client.api('/applications')
    .version('beta')
    .post(application);

```