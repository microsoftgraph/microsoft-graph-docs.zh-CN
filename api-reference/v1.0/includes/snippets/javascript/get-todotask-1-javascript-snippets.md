---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61fd13461811ffbffc61e5874fe1f19dbeb52006
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963476"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let todoTask = await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .get();

```