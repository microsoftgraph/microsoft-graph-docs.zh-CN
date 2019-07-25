---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4fe3bde5536979c95d3d6f6a03761ed1d92df87a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const replyAll = {
  comment: "comment-value"
};

let res = await client.api('/me/messages/{id}/replyAll')
    .post(replyAll);

```