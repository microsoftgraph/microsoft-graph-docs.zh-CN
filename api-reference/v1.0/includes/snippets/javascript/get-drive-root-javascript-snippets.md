---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3db31f97ed1d7e2c04a0a40e79326e643fcef0c6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614163"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root')
    .get();

```