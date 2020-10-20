---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b79cfc50b54a5babda4482320e7dd8924190524
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions/{id}')
    .version('beta')
    .delete();

```