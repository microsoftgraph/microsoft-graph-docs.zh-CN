---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 97d3e2af844f9d0d25d60010ce7dae73065f6258
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    driveId: "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    id: "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  name: "contoso plan (copy).txt"
};

let res = await client.api('/me/drive/items/{item-id}/copy')
    .post(driveItem);

```