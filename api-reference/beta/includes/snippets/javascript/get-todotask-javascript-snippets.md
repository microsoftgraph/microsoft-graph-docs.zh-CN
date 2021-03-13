---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aed9a8dcd7be56983489d8381a8b3fc0903598c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785971"
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