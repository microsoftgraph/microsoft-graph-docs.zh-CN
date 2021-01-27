---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdbfe6e98743651c566c3d85e0c05dc3997be0a4
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/termStore/groups/{groupId}/sets/{setId}/terms/{termId}')
    .version('beta')
    .get();

```