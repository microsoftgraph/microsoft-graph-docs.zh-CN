---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97d3e2af844f9d0d25d60010ce7dae73065f6258
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614885"
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