---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5af47a15f49a64234aa77197e4b5a06cb28f7fd1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{class-id}/teachers/{teacher-id}')
    .delete();

```