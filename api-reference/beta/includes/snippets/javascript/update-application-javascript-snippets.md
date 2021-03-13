---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34a81828b56029cf08b2f25d252cb79e4ff683f9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: 'New display name'
};

await client.api('/applications/{id}')
    .version('beta')
    .update(application);

```