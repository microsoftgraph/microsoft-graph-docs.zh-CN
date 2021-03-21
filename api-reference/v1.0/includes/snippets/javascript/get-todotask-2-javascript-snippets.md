---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 301c43162aed19a04755404c07b53c5f1ee93ad5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963370"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks')
    .get();

```