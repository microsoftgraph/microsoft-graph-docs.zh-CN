---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1af37b5a5efcef2033955a8d17f8d79b1deb1b76
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4')
    .version('beta')
    .delete();

```