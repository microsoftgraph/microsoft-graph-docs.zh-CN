---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38869e94f85ea8646b456f78197cb3b6d0665d3c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: "id-value",
  groupId: "groupId-value",
  renameAs: "renameAs-value"
};

let res = await client.api('/me/onenote/sections/{id}/copyToSectionGroup')
    .post(onenoteOperation);

```