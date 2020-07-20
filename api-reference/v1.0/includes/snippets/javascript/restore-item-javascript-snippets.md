---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c7f6ecd41d7c05bf0e5a6e81d7a0d8e118f8a1f
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    id: "String",
  },
  name: "String"
};

let res = await client.api('/me/drive/items/{item-id}/restore')
    .version('beta')
    .post(driveItem);

```