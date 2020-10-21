---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0175722425643281be38475b34c70a6b0e26b78f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/supportedLanguages')
    .get();

```