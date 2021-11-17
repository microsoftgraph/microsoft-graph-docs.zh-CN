---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6ee394043944db45af242a34451e99ce8d56c1e2a65167c0975cafeb6649610
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278752"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks')
    .version('beta')
    .get();

```