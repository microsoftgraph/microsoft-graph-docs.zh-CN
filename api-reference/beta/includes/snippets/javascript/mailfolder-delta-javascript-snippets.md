---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76646b569e9c45480d0ac67ff5e62f5c2c9c48f3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/delta')
    .version('beta')
    .get();

```