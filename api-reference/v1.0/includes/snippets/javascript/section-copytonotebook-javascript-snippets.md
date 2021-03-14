---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce943fcc08b029437569cbbd7305ec499af702dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: 'id-value',
  groupId: 'groupId-value',
  renameAs: 'renameAs-value'
};

await client.api('/me/onenote/sections/{id}/copyToNotebook')
    .post(onenoteOperation);

```