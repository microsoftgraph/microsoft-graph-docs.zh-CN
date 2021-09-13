---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c4876a1b165e51c70a8c68d5325b1255e06706a21b10793cfc32090f902fa99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .delete();

```