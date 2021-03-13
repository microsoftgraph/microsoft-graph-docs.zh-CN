---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3658ac89b9eabc30976e1fae94c32a4e02d06df
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .version('beta')
    .delete();

```