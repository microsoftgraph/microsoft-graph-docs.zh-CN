---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaa0d219636df70dfa4181519e9e42894184d32b418649af00e2dbb4a3d1dbd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  groupId: 'groupId-value',
  renameAs: 'renameAs-value'
};

await client.api('/me/onenote/notebooks/{id}/copyNotebook')
    .version('beta')
    .post(onenoteOperation);

```