---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e258d8bbadec8e86d12101245d9851bd18846bd5154337aeb3ae5ae53b6ac44b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162320"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let todoTask = await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .get();

```