---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70b47e0e3fa3676a671f785db477c05d1c02d219f1bd14a6b8b742e7083a754c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333460"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks')
    .get();

```