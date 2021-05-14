---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a9467d87bf949ed2a48f07bea8934323a441bf3
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationClass = await client.api('/education/classes/{educationClassId}')
    .get();

```