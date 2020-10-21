---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f09b7b1cef74694971e229244e5cf4c45719b3b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscribedSkus/{id}')
    .get();

```