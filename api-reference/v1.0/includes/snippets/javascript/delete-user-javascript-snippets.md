---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9d575911b7cfa289b301d4d98c0fe74ec3ba326
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{user-id}')
    .delete();

```