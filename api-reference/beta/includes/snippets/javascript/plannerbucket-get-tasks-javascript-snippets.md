---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5892a86cc5a06ba5a38ea89d9dcd9d19a5d80429
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637459"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/tasks')
    .version('beta')
    .get();

```