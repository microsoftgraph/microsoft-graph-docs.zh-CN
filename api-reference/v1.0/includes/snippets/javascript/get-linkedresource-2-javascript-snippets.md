---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87eb002bda8aba36684e7611b96ceba095aeb3b61675cedd66a9dc4a4a350e79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279647"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let linkedResources = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources')
    .get();

```