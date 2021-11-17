---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbd2b183e020d9477b498a04145fad6c5c5a079cf2cb355e92418cc771b27a3d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let todoTask = await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .version('beta')
    .get();

```