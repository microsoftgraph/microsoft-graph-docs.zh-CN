---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5f85aca9f4f74ca3f900a24ff31640072071f40836638bbe18e3123219de72b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTaskDetails = await client.api('/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details')
    .version('beta')
    .get();

```