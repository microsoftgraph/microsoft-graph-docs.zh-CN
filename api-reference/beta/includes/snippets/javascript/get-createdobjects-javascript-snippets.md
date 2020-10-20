---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53d23056d9832a9ef5935564785e75741a7f341b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/createdObjects')
    .version('beta')
    .get();

```