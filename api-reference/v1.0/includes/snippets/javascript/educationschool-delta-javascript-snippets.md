---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db9aa20349ad1708a7d0fda8ddb9a8c30ea0a7da
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/schools/delta')
    .get();

```