---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5779ffe1b93bd6ba86f6f9b21e17670b8a193d75
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636573"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "Shared legal agreements"
};

let res = await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .update(driveItem);

```