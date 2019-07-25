---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c26086b587993a7d446c67582bd2786dea5d170e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734928"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    path: "/drive/root:/Documents"
  },
  name: "Copy of LargeFolder1"
};

let res = await client.api('/me/drive/items/{folder-item-id}/copy')
    .version('beta')
    .post(driveItem);

```