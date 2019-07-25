---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 60c0c0a197b0b8aa7d9435f0e0ff5a689cd4e191
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720432"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details')
    .version('beta')
    .get();

```