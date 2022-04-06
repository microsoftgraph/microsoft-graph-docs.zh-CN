---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79d559a16df7b5f606bc422d3138009f512eb5bf
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'Shared legal agreements'
};

await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .update(driveItem);

```