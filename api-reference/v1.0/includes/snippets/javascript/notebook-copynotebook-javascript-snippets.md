---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b05e36cbb6881aa8746e62f8f55e90a07586e5ead65df1ae683ee87728dfbec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409506"
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
    .post(onenoteOperation);

```