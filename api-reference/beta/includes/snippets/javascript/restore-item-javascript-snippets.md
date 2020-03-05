---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c7f6ecd41d7c05bf0e5a6e81d7a0d8e118f8a1f
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402095"
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