---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4ebf1f17a68d988fe2c9d9f0ae75699bd18bf331
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  directorySetting: {
    displayName: "displayName-value",
    templateId: "templateId-value",
    values: [
      {
        name: "name-value",
        value: "value-value"
      }
    ]
  }
};

let res = await client.api('/groups/{id}/settings')
    .version('beta')
    .post(directorySetting);

```