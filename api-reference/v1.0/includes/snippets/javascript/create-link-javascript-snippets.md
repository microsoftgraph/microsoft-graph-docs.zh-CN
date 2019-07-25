---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 214953ab3b3bcba417f4f92915bf8e3da90c5d00
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: "view",
  scope: "anonymous"
};

let res = await client.api('/me/drive/items/{item-id}/createLink')
    .post(permission);

```