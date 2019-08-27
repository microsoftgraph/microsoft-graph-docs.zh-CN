---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8fd72efe943c26eb532b5687d5e83cc15eac7c5b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636494"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/users/{id}"
};

let res = await client.api('/groups/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```