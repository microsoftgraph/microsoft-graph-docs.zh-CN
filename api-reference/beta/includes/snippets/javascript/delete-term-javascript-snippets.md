---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fb17f59b3e80847a03f69bc7e19a8fbf6cc17a2
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/termStore/sets/{setId}/terms/{termId}')
    .version('beta')
    .delete();

```