---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dcdeb38adc6c648a3c8c3c745dff50113ede111964cd52de1158e3bcf3b2cfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/buckets/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/tasks')
    .version('beta')
    .get();

```