---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f42a1074a9bb8a978512529ecf771d3ce786dd1
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/ownedObjects')
    .get();

```