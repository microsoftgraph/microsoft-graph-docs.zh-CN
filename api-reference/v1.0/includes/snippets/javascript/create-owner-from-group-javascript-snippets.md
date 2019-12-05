---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c848ccf584540cb9398dde135ade8e869d28b1b1
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/users/{id}"
};

let res = await client.api('/groups/{id}/owners/$ref')
    .post(directoryObject);

```