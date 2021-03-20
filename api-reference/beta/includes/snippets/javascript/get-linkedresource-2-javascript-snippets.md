---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be8021f81f190c859ec9c5bd4f2b18e5d2fed8c3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942086"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let linkedResources = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources')
    .version('beta')
    .get();

```