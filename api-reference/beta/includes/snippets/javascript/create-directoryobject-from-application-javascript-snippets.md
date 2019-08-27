---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9485911925da47d31bbf7f3b95dd1e5a825baf44
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
@odata.id: "https://graph.microsoft.com/beta/directoryObjects/{id}"
};

let res = await client.api('/applications/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```