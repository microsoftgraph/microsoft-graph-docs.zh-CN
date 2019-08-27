---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 14552e47ec9d12407cac91a0979276617b6ba12c
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  id: "123456!87"
};

let res = await client.api('/drive/bundles/{bundle-id}/children')
    .version('beta')
    .post(driveItem);

```