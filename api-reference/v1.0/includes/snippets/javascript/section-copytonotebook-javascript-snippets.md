---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26f48e9a296ce567a20638bd33191f45c8e5bf873465c699e364da9c33cb4118
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902222"
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