---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dc9500cb4bff356a3a85a6bbc714405d37e8e2a
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}/schools')
    .get();

```