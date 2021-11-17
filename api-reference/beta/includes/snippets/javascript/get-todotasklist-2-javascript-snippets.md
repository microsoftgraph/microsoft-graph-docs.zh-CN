---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33971bfa474d19c7475b2674dc1c50c8706f94478b97c0cdcc6e052cb62bae2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let todoTaskList = await client.api('/me/todo/lists/AAMkADIyAAAAABrJAAA=')
    .version('beta')
    .get();

```