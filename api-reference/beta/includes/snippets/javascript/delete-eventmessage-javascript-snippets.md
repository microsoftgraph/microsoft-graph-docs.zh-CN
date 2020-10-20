---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09be6cce37496400b52c3e4798f2d33113feec0b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606071"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}')
    .version('beta')
    .delete();

```